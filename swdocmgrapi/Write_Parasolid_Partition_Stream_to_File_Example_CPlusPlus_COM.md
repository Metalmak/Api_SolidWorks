<!-- source: swdocmgrapi/Write_Parasolid_Partition_Stream_to_File_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS Document Manager API Help

# Write Parasolid Partition Stream to File Example (C++)

This example shows how to write a Parasolid partition stream to a file
using the SOLIDWORKS Document Manager API.

#import 'C:\Program Files\Common Files\SOLIDWORKS Shared\swdocumentmgr.dll'
 raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids //Change as necessary

wchar\_t\* filename = "87-part.sldprt"

wchar\_t\* outputDir = "c:\\caddocs\\";

ISwDMClassFactoryPtr swClassFact;

 swClassFact.CreateInstance(

 \_\_uuidof(SwDMClassFactory)
);

 if
(!(ISwDMClassFactory\*)swClassFact)

 return
0;

 ISwDMApplicationPtr
swDocMgr(

 swClassFact->GetApplication("your\_license\_key")
); //Specify your license
key

 if
(!(ISwDMApplication\*)swDocMgr)

 return
0;

 SwDmDocumentOpenError
error;

 ISwDMDocumentPtr
swDoc( swDocMgr->GetDocument(

 filename,
swDmDocumentPart, TRUE, &error ) );

 if
(!(ISwDMDocument\*)swDoc)

 return
0;

 ISwDMConfigurationMgrPtr
swCfgMgr(

 swDoc->ConfigurationManager );

 if
(!(ISwDMConfigurationMgr\*)swCfgMgr)

 return
0;

 \_variant\_t
names( swCfgMgr->GetConfigurationNames()
);

 SAFEARRAY\*
nameArray = names.parray;

 for
(int i=0; i<nameArray->rgsabound[0].cElements; ++i)

 {

 \_bstr\_t
str( ((BSTR\*)(nameArray->pvData))[i] );

 ISwDMConfigurationPtr
swCfg(

 swCfgMgr->GetConfigurationByName(str) );

 ISwDMConfiguration2\*
pswCfg2;

 if
(swCfg)

swCfg->QueryInterface( \_\_uuidof(ISwDMConfiguration2),
(void \*\*)&pswCfg2 );

else

return 0;

 {

 CString
dir( outputDir );

 dir
+= "\\";

 dir
+= str;

 dir
+= ".xmp\_bin";

 pswCfg2->GetPartitionStream( (LPCTSTR)dir );

 }

 }
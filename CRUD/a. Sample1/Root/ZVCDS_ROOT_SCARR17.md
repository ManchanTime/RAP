```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'ROOT CDS Practice'
@Metadata.ignorePropagatedAnnotations: true
//@Metadata.allowExtensions: true

define root view entity ZVCDS_ROOT_SCARR17 
    as select from zcl1scarr17
{
    key carrid   as Carrid,
        carrname as Carrname,
        currcode as Currcode,
        url      as Url
}

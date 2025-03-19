```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Book root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SBOOK17 as select from sbook {

    // Key Fields
    key carrid   as Carrid,
    key connid   as Connid,
    key fldate   as Fldate,
    key bookid   as Bookid,

    // Customer Information
    customid as Customid,
    custtype as Custtype,

    // Additional Information
    smoker   as Smoker
}

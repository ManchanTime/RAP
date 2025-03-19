```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Book projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_SBOOK17 as projection on ZVCDS_ROOT_SBOOK17 {

    // Key Fields
    key Carrid,
    key Connid,
    key Fldate,
    key Bookid,

    // Customer Information
    Customid,
    Custtype,

    // Additional Information
    Smoker
}

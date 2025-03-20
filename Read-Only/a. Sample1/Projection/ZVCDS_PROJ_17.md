```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Schedule projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_SPFLI17 as projection on ZVCDS_ROOT_SPFLI17 {

    // Key Fields
    key Carrid,
    key Connid,
    
    // Departure Information
    Countryfr,
    Cityfrom,
    Airpfrom,

    // Arrival Information
    Countryto,
    Cityto,
    Airpto
}

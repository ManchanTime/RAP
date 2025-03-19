```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Airline join view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_JOIN_AIR17 as projection on ZVCDS_ROOT_JOIN_AIR17 {

    // Key Fields
    key Carrid,
    key Connid,

    // Airline Information
    Carrname,
    Currcode,
    Url,

    // Departure Information
    Countryfr,
    Cityfrom,
    Airpfrom,

    // Arrival Information
    Countryto,
    Cityto,
    Airpto
}

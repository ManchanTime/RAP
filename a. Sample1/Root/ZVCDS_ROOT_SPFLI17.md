```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Schedule root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SPFLI17 as select from spfli {
  
  // Key Fields
  key carrid    as Carrid,
  key connid    as Connid,
  
  // Departure Information
  countryfr as Countryfr,
  cityfrom  as Cityfrom,
  airpfrom  as Airpfrom,
  
  // Arrival Information
  countryto as Countryto,
  cityto    as Cityto,
  airpto    as Airpto
}

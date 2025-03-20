```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Flight projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_SFLIGHT17 as projection on ZVCDS_ROOT_SFLIGHT17 {

    // Key Fields
    key Carrid,
    key Connid,
    key Fldate,

    // Pricing Information
    Price,
    
    // Currency Information
    Currency,
    
    // Plane Information
    Planetype,
    
    // Seating Information
    Seatsmax,
    Seatsocc
}

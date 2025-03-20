```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Flight root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_SFLIGHT17 as select from sflight {

    // Key Fields
    key carrid    as Carrid,
    key connid    as Connid,
    key fldate    as Fldate,
    
    // Pricing Information
    @Semantics.amount.currencyCode: 'Currency'
    price     as Price,
    
    // Currency Information
    currency  as Currency,
    
    // Plane Information
    planetype as Planetype,
    
    // Seating Information
    seatsmax  as Seatsmax,
    seatsocc  as Seatsocc
}

```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Flight join projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_JOIN_FLIGHT17 as projection on ZVCDS_ROOT_JOIN_FLIGHT17 {

    // Key Fields
    key Carrid,
    key Connid,
    key Fldate,
    key Bookid,

    // Customer Information
    Customid,
    Custtype,
    Smoker,

    // Booking Information
    OrderDate,
    Counter,
    Agencynum,
    Cancelled,
    Reserved,

    // Passenger Information
    Passname,
    Passform,
    Passbirth,

    // Flight Information
    Price,
    Currency,
    Planetype,
    Seatsmax,
    Seatsocc
}

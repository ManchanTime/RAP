```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Flight join root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_JOIN_FLIGHT17 as select from sflight as a
    inner join sbook as b
    on  a.carrid = b.carrid
    and a.connid = b.connid
    and a.fldate = b.fldate {

    // Key Fields
    key b.carrid     as Carrid,
    key b.connid     as Connid,
    key b.fldate     as Fldate,
    key b.bookid     as Bookid,

    // Customer Information
    b.customid   as Customid,
    b.custtype   as Custtype,
    b.smoker     as Smoker,

    // Booking Information
    b.order_date as OrderDate,
    b.counter    as Counter,
    b.agencynum  as Agencynum,
    b.cancelled  as Cancelled,
    b.reserved   as Reserved,

    // Passenger Information
    b.passname   as Passname,
    b.passform   as Passform,
    b.passbirth  as Passbirth,

    // Flight Information
    @Semantics.amount.currencyCode: 'Currency'
    a.price      as Price,
    a.currency   as Currency,
    a.planetype  as Planetype,
    a.seatsmax   as Seatsmax,
    a.seatsocc   as Seatsocc
}

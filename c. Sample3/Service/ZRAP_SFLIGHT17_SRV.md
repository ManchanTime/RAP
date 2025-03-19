``` abap
@EndUserText.label: 'RAP Flight OData service'

define service ZRAP_SFLIGHT17_SRV {

    // Expose Flight Projection
    expose ZVCDS_PROJ_SFLIGHT17 as flight;

    // Expose Booking Projection
    expose ZVCDS_PROJ_SBOOK17 as book;
}

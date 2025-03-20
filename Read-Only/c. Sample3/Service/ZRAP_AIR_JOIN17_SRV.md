```abap
@EndUserText.label: 'RAP AIR JOIN OData Service'

define service ZRAP_AIR_JOIN17_SRV {

    // Expose Airline Projection
    expose ZVCDS_PROJ_JOIN_AIR17 as air;

    // Expose Flight Projection
    expose ZVCDS_PROJ_JOIN_FLIGHT17 as flight;
}

```abap
@EndUserText.label: 'RAP Airline master OData service'

define service ZRAP_SCARR17_SRV {
    expose ZVCDS_PROJ_SCARR16 as airline;
    expose ZVCDS_ROOT_SPFLI17 as schedule;
}

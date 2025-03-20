```abap
@EndUserText.label: 'RAP Airline master OData service'

define service ZVCDS_PROJ_SCARR16_SRV
{
    expose ZVCDS_PROJ_SCARR16 as AirlineSet;
}

```abap
@EndUserText.label: 'RAP Material service'

define service ZVCDS_PROJ_MAT17_SRV
{
    expose ZVCDS_PROJ_MAT17 as MaterialSet;
}

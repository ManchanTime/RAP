```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Material projection view'
@Metadata.ignorePropagatedAnnotations: true
@Metadata.allowExtensions: true

define root view entity ZVCDS_PROJ_MAT17
    as projection on ZVCDS_ROOT_MAT17
{
    key Matnr,
    key Werks,
    key Lgort,

        Mtart,
        Matkl,
        Menge,
        Meins,
        Wrbtr,
        Waers,
        Lvorm
}

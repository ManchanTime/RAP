```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Material root view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_ROOT_MAT17
    as select from ztcl1_17_01
{
    key matnr as Matnr,
    key werks as Werks,
    key lgort as Lgort,

        mtart as Mtart,
        matkl as Matkl,

    @Semantics.quantity.unitOfMeasure: 'Meins'
        menge as Menge,
        meins as Meins,

    @Semantics.amount.currencyCode: 'Waers'
        wrbtr as Wrbtr,
        waers as Waers,

        lvorm as Lvorm
}

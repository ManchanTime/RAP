```abap
@AccessControl.authorizationCheck: #NOT_REQUIRED
@EndUserText.label: 'RAP Airline master projection view'
@Metadata.ignorePropagatedAnnotations: true

define root view entity ZVCDS_PROJ_SCARR16
    as projection on ZVCDS_ROOT_SCARR17 {
        key Carrid,
            Carrname,
            Currcode,
            Url
    }

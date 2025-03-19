```abap
@EndUserText.label: 'RAP Airline master OData service'

define service ZRAP_SCARR17_SRV {  
    // Expose Airline Projection
    expose ZVCDS_PROJ_SCARR16 as airline;  
    
    // Expose Schedule Root
    expose ZVCDS_ROOT_SPFLI17 as schedule;
}

// Scarr 서비스에 Spfli 붙이기

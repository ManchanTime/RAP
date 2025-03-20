```abap
@Metadata.layer: #CORE

@UI: {
    headerInfo: {
        typeName: 'AirlineInfo',
        typeNamePlural: 'Airline master',
        title: { value:'AirlineData' },
        description : { value: 'AirlineMaster' }
    }
}

annotate view ZVCDS_PROJ_SCARR16 with
{
    @UI.facet: [
        {
            id: 'AirlineInfo',
            purpose: #STANDARD,
            type: #IDENTIFICATION_REFERENCE,
            label: 'AirlineInfo',
            position: 10
        }
    ]

    @UI: {
        lineItem: [
            {
                position: 10,
                label: 'Airline Code',
                importance: #HIGH
            }
        ],
        identification: [
            {
                position: 10,
                label: '항공사 코드',
                importance: #HIGH
            }
        ]
    }
    Carrid;

    @UI: {
        lineItem: [
            {
                position: 10,
                label: 'Airline Name',
                importance: #HIGH
            }
        ],
        identification: [
            {
                position: 10,
                label: '항공사 이름',
                importance: #HIGH
            }
        ]
    }
    Carrname;

    @UI: {
        lineItem: [
            {
                position: 10,
                label: 'Currency Code',
                importance: #HIGH
            }
        ],
        identification: [
            {
                position: 10,
                label: '항공사 통화키',
                importance: #HIGH
            }
        ]
    }
    Currcode;

    @UI: {
        lineItem: [
            {
                position: 10,
                label: 'Airline Url',
                importance: #HIGH
            }
        ],
        identification: [
            {
                position: 10,
                label: 'Homepage URL',
                importance: #HIGH
            }
        ]
    }
    Url;
}

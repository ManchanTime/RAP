```abap
@Metadata.layer: #CORE

@UI: {
    headerInfo: {
        typeName: 'MatInfor',
        typeNamePlural: 'MatInformation',
        title: { value: 'MatInfor' },
        description: { value: 'MaterialDescription' }
    }
}

annotate view ZVCDS_PROJ_MAT17 with
{
    @UI.facet: [
        {
            id: 'MainInfor',
            purpose: #STANDARD,
            type: #IDENTIFICATION_REFERENCE,
            label: 'MainInfor',
            position: 10
        }
    ]

    // Material Code
    @UI: {
        lineItem: [
            { position: 10, label: 'Material Code', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '자재코드', importance: #HIGH }
        ]
    }
    Matnr;

    // Plant
    @UI: {
        lineItem: [
            { position: 10, label: 'Plant', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '플랜트', importance: #HIGH }
        ]
    }
    Werks;

    // Storage location
    @UI: {
        lineItem: [
            { position: 10, label: 'Storage location', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '저장위치', importance: #HIGH }
        ]
    }
    Lgort;

    // Material type
    @UI: {
        lineItem: [
            { position: 10, label: 'Material type', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '자재 타입', importance: #HIGH }
        ]
    }
    Mtart;

    // Material Group
    @UI: {
        lineItem: [
            { position: 10, label: 'Material Group', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '자재 그룹', importance: #HIGH }
        ]
    }
    Matkl;

    // Quantity
    @UI: {
        lineItem: [
            { position: 10, label: 'Quantity', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '수량', importance: #HIGH }
        ]
    }
    Menge;

    // Base Unit of Measure
    @UI: {
        lineItem: [
            { position: 10, label: 'Base Unit of Measure', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '단위', importance: #HIGH }
        ]
    }
    Meins;

    // Amount in document currency
    @UI: {
        lineItem: [
            { position: 10, label: 'Amount in document currency', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '외화 금액', importance: #HIGH }
        ]
    }
    Wrbtr;

    // Currency Key
    @UI: {
        lineItem: [
            { position: 10, label: 'Currency Key', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '통화키', importance: #HIGH }
        ]
    }
    Waers;

    // Deletion Indicator
    @UI: {
        lineItem: [
            { position: 10, label: 'Deletion Indicator', importance: #HIGH }
        ],
        identification: [
            { position: 10, label: '삭제 플래그', importance: #HIGH }
        ]
    }
    Lvorm;
}

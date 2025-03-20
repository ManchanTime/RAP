```abap
managed; // implementation in class zbp_vcds_root_mat17 unique;

define behavior for ZVCDS_ROOT_MAT17    // alias <alias_name>
    persistent table ztcl1_17_01
    lock master
    // authorization master (instance)
    // etag master <field_name>
{
    create;
    update;
    delete;

    mapping for ztcl1_17_01 corresponding
    {
        Matnr = matnr;
        Werks = werks;
        Lgort = lgort;
        Mtart = mtart;
        Matkl = matkl;
        Menge = menge;
        Meins = meins;
        Wrbtr = wrbtr;
        Waers = waers;
        Lvorm = lvorm;
    }
}

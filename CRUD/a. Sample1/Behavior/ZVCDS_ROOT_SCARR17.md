```abap
managed; // implementation in class zbp_vcds_root_scarr17 unique;

define behavior for ZVCDS_ROOT_SCARR17    // alias <alias_name>
    persistent table zcl1scarr17
    lock master
    // authorization master (instance)
    // etag master <field_name>
{
    create;
    update;
    delete;

    mapping for zcl1scarr17 corresponding
    {
        Carrid   = carrid;
        Carrname = carrname;
        Currcode = currcode;
        Url      = url;
    }
}

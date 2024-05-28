# Comparing `tmp/ezdxf-1.3.0rc0.zip` & `tmp/ezdxf-1.3.1b0.zip`

## zipinfo {}

```diff
@@ -1,860 +1,870 @@
-Zip file size: 2194990 bytes, number of entries: 858
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/LICENSE
--rw-rw-rw-  2.0 fat      329 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/MANIFEST.in
--rw-rw-rw-  2.0 fat    10111 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/PKG-INFO
--rw-rw-rw-  2.0 fat     2527 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/pyproject.toml
--rw-rw-rw-  2.0 fat     7479 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/README.md
--rw-rw-rw-  2.0 fat       74 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/requirements.txt
--rw-rw-rw-  2.0 fat       42 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/setup.cfg
--rw-rw-rw-  2.0 fat     2140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     1339 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_acis_entites.py
--rw-rw-rw-  2.0 fat     4686 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4153 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      577 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_appsettings.py
--rw-rw-rw-  2.0 fat      871 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1299 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py
--rw-rw-rw-  2.0 fat     1558 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      905 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     7747 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     2347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_xref_load_acis.py
--rw-rw-rw-  2.0 fat     3060 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat    56494 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip
--rw-rw-rw-  2.0 fat     1592 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat    19533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf
--rw-rw-rw-  2.0 fat    19506 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf
--rw-rw-rw-  2.0 fat    19291 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf
--rw-rw-rw-  2.0 fat    19383 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4841 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19886 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7872 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    17062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    33508 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22334 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    55319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat     2475 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py
--rw-rw-rw-  2.0 fat    16254 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    14519 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10366 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107528 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat    20554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    35308 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    31442 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat     3926 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/revcloud.py
--rw-rw-rw-  2.0 fat    11250 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/select.py
--rw-rw-rw-  2.0 fat    12848 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    18280 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/xclip.py
--rw-rw-rw-  2.0 fat    65739 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10898 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     3138 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat    11502 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    14048 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat      252 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/constants.h
--rw-rw-rw-  2.0 fat    11844 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3161 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23976 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23703 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     4705 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx
--rw-rw-rw-  2.0 fat     1719 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23377 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6398 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      888 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5489 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6731 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2985 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4093 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13189 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      120 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31454 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22005 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    38393 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8946 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16307 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22301 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7605 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12768 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3335 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat     9975 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1249 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    21111 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     6896 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py
--rw-rw-rw-  2.0 fat     2214 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1366 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     9265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat    11113 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1756 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat     7391 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py
--rw-rw-rw-  2.0 fat     7753 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py
--rw-rw-rw-  2.0 fat    44576 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1877 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    20834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py
--rw-rw-rw-  2.0 fat    20101 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py
--rw-rw-rw-  2.0 fat    18871 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    13209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9862 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    32445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py
--rw-rw-rw-  2.0 fat    40194 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    18036 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py
--rw-rw-rw-  2.0 fat    11577 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22713 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat    16434 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    16222 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1194 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2559 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat    13443 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      561 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat    16079 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat    11766 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5615 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     6222 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    19435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     5729 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    21463 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat     2850 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py
--rw-rw-rw-  2.0 fat    29778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4996 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    27092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     8881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10586 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50111 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7929 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat     3214 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py
--rw-rw-rw-  2.0 fat    24981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48717 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35043 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23813 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    40656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    27114 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23679 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13910 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4138 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23747 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4838 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    27125 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    28148 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    28698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14278 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    13070 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    19055 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    17444 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57437 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2151 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16525 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40126 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10485 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat     7990 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py
--rw-rw-rw-  2.0 fat    23810 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8382 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat     1341 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/temporary_transform.py
--rw-rw-rw-  2.0 fat    17633 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3617 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14452 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28360 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7958 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8531 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    26337 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    18620 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      288 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_synonyms.py
--rw-rw-rw-  2.0 fat     1175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35414 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7244 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    32460 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16560 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     2715 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    16997 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7152 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    14509 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14325 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat    11054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12000 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17303 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    15532 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9310 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2458 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    53170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9135 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    33170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    11618 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26176 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1273 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    21723 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    13190 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py
--rw-rw-rw-  2.0 fat    27210 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15934 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11827 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     4815 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat    12135 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3539 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    17116 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     6710 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    11876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat    12477 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2548 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24812 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    22757 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25882 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     1978 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    31043 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     5868 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    18224 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10129 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat    10125 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17745 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    51443 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    25780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    65258 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22557 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16492 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11937 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    61373 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26565 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20440 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat    15737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7613 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2325 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1224 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6187 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    66061 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3116 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     4413 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       46 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    10111 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      316 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    33000 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5667 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8688 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8797 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     2581 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
--rw-rw-rw-  2.0 fat     1500 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat     1947 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
--rw-rw-rw-  2.0 fat    11689 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2622 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4679 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9199 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     1876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py
--rw-rw-rw-  2.0 fat     2141 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
--rw-rw-rw-  2.0 fat     2231 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     6487 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     8628 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5916 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6914 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7345 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12226 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py
--rw-rw-rw-  2.0 fat     7614 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py
--rw-rw-rw-  2.0 fat     1854 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
--rw-rw-rw-  2.0 fat     4215 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
--rw-rw-rw-  2.0 fat     1936 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11333 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4850 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat     1039 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
--rw-rw-rw-  2.0 fat   112800 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     2665 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      657 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    18181 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9361 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4752 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2469 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12357 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43259 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    48174 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     7186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat    17771 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     1206 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py
--rw-rw-rw-  2.0 fat     1400 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py
--rw-rw-rw-  2.0 fat    11705 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py
--rw-rw-rw-  2.0 fat     1264 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7503 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14661 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2829 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9709 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    14118 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     6332 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
--rw-rw-rw-  2.0 fat    10913 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     7712 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10869 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10900 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10354 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    20154 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    11561 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     9001 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3212 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11654 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1266 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
--rw-rw-rw-  2.0 fat    17333 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py
--rw-rw-rw-  2.0 fat     7980 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py
--rw-rw-rw-  2.0 fat     1553 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     4459 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    34121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27365 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3278 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11887 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12491 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    11204 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    12549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     9101 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     2898 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py
--rw-rw-rw-  2.0 fat     4229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    13751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15655 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1376 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat     5284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     2014 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
--rw-rw-rw-  2.0 fat     3158 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py
--rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1463 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4773 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-858 files, 8903508 bytes uncompressed, 2038206 bytes compressed:  77.1%
+Zip file size: 2210198 bytes, number of entries: 868
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/LICENSE
+-rw-rw-rw-  2.0 fat      329 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/MANIFEST.in
+-rw-rw-rw-  2.0 fat    10110 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/PKG-INFO
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/pyproject.toml
+-rw-rw-rw-  2.0 fat     7479 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/README.md
+-rw-rw-rw-  2.0 fat       74 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/requirements.txt
+-rw-rw-rw-  2.0 fat       42 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/setup.cfg
+-rw-rw-rw-  2.0 fat     2140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     1339 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_acis_entites.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4153 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      577 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_appsettings.py
+-rw-rw-rw-  2.0 fat      871 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1299 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     7747 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     2347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat    56494 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/dynblks.zip
+-rw-rw-rw-  2.0 fat     1592 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat    19533 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf
+-rw-rw-rw-  2.0 fat    19506 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf
+-rw-rw-rw-  2.0 fat    19291 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf
+-rw-rw-rw-  2.0 fat    19383 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4841 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7872 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    17062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    33508 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22334 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    55248 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat     2475 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py
+-rw-rw-rw-  2.0 fat    21292 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/edgeminer.py
+-rw-rw-rw-  2.0 fat     5441 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/edgesmith.py
+-rw-rw-rw-  2.0 fat    16254 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    14519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10366 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat      658 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/messenger.py
+-rw-rw-rw-  2.0 fat      272 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/msgtypes.py
+-rw-rw-rw-  2.0 fat    20554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     3030 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    35308 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    31442 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat     3926 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/revcloud.py
+-rw-rw-rw-  2.0 fat    11250 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/select.py
+-rw-rw-rw-  2.0 fat    12848 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    18280 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/xclip.py
+-rw-rw-rw-  2.0 fat    65739 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     3138 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat    11502 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    14048 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat      252 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/constants.h
+-rw-rw-rw-  2.0 fat    11844 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3161 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     4705 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx
+-rw-rw-rw-  2.0 fat     1719 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23377 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6398 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      938 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     1792 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/cache.py
+-rw-rw-rw-  2.0 fat     5489 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6731 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4093 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    15566 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13189 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      247 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/type_hints.py
+-rw-rw-rw-  2.0 fat      120 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26766 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31464 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22005 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    38393 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8946 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16364 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22301 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7605 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12768 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3335 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat     9975 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1249 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1366 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     9265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat    11113 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1756 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat     7391 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat     7753 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py
+-rw-rw-rw-  2.0 fat    44576 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    20834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    20101 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py
+-rw-rw-rw-  2.0 fat    18871 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    13209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9862 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    32445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py
+-rw-rw-rw-  2.0 fat    40194 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    18036 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    11577 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22713 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    16434 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    16222 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13443 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      561 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11766 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     5710 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    21579 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat     2850 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py
+-rw-rw-rw-  2.0 fat    30267 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4996 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    27092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     8881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10586 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    51025 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7929 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat     3214 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/copy.py
+-rw-rw-rw-  2.0 fat    24981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48717 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35043 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23813 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    40587 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    27114 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    16471 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23679 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13910 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4138 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23747 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4838 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    27125 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    28148 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    28698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14358 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    13070 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    19055 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    17444 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57437 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2151 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16978 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40126 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10485 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat     7990 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py
+-rw-rw-rw-  2.0 fat    23810 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat     1341 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py
+-rw-rw-rw-  2.0 fat    17633 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3617 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14452 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28360 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7958 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8531 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    26337 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    18620 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      288 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_synonyms.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35414 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7244 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16964 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    32460 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16560 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     2715 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    16997 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7152 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    14509 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14325 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat    11054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12000 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17303 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    15532 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9310 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2458 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    53170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9135 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    33170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    11618 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26176 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1273 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    21723 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    13190 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/legacy.py
+-rw-rw-rw-  2.0 fat    27210 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15934 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     4815 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat    12135 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3539 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    17116 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     6710 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    11876 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat    12477 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2548 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24812 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    22757 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25882 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     1978 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    31293 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    18224 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10129 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat    10125 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17745 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    51443 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    25780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    65258 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22287 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    17369 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11937 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    61373 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26565 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20440 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat    15737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7613 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2325 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1224 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6187 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    66061 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     4413 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       46 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    10110 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      316 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    33328 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5667 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8688 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8797 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     2581 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat     1947 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2622 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4679 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     1876 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py
+-rw-rw-rw-  2.0 fat     2141 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     6487 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     8628 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5916 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6914 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7345 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     3104 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12226 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py
+-rw-rw-rw-  2.0 fat     7614 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
+-rw-rw-rw-  2.0 fat     4215 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
+-rw-rw-rw-  2.0 fat     1936 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11333 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     7274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4850 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2340 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     8058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat     7813 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     2665 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      657 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    18181 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9361 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4752 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2469 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12357 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7858 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43259 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    48174 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     7186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat    17771 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     1206 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py
+-rw-rw-rw-  2.0 fat     1400 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py
+-rw-rw-rw-  2.0 fat    11705 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_545_acis_cache.py
+-rw-rw-rw-  2.0 fat    13061 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_546_edgeminer.py
+-rw-rw-rw-  2.0 fat     3413 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_547_edgesmith.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7503 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14661 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2829 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9709 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    14118 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     6332 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     7712 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10869 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10900 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10354 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    20154 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    11561 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     9001 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3212 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11654 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1266 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+-rw-rw-rw-  2.0 fat    17333 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     7980 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     1553 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     4459 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    34121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27365 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3278 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11887 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    13038 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    16011 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    11204 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    12549 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     9101 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    13751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py
+-rw-rw-rw-  2.0 fat     3388 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1463 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4773 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     1666 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_1078_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+868 files, 8966146 bytes uncompressed, 2053454 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -1,2575 +1,2605 @@
-Filename: ezdxf-1.3.0rc0/
+Filename: ezdxf-1.3.1b0/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/
+Filename: ezdxf-1.3.1b0/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/
+Filename: ezdxf-1.3.1b0/src/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/
+Filename: ezdxf-1.3.1b0/tests/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/LICENSE
+Filename: ezdxf-1.3.1b0/LICENSE
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/MANIFEST.in
+Filename: ezdxf-1.3.1b0/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/PKG-INFO
+Filename: ezdxf-1.3.1b0/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/pyproject.toml
+Filename: ezdxf-1.3.1b0/pyproject.toml
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/README.md
+Filename: ezdxf-1.3.1b0/README.md
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/requirements.txt
+Filename: ezdxf-1.3.1b0/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/setup.cfg
+Filename: ezdxf-1.3.1b0/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/setup.py
+Filename: ezdxf-1.3.1b0/setup.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/
+Filename: ezdxf-1.3.1b0/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/conftest.py
+Filename: ezdxf-1.3.1b0/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_acad_table.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_acis_entites.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_acis_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_appsettings.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_document_guid.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_geo.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_groups.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_launcher.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_odafc.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_r12export.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_r12strict.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_r12writer.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_recover.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/test_xref_load_acis.py
+Filename: ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip
+Filename: ezdxf-1.3.1b0/integration_tests/data/dynblks.zip
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/groups.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/
+Filename: ezdxf-1.3.1b0/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/appsettings.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/audit.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/bbox.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/colors.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/commands.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/comments.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/disassemble.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/document.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entitydb.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/edgeminer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/enums.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/edgesmith.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/explode.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/eztypes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/groupby.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/npshapes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/protocols.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/messenger.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/py.typed
+Filename: ezdxf-1.3.1b0/src/ezdxf/msgtypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/query.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/queryparser.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/r12strict.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/recover.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/reorder.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/revcloud.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/select.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/transform.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/units.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/upright.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/urecord.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/select.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/version.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/xclip.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/xref.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/zoom.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/_options.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/__main__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/constants.h
+Filename: ezdxf-1.3.1b0/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/constants.h
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/api.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/const.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/cache.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/block.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/copy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/image.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/light.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/line.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/material.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/point.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/table.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/temporary_transform.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/text.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/view.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_synonyms.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_synonyms.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/arc.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/box.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/circle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/line.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/legacy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/shape.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/commands.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/converter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/path.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/tools.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/curves.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/forms.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/leader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/point.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/trace.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/header.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/table.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/test.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/
+Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/conftest.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.3.1b0/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/conftest.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_545_acis_cache.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_546_edgeminer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_547_edgesmith.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_1078_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py
+Comment: 
+
+Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.3.0rc0/LICENSE` & `ezdxf-1.3.1b0/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/PKG-INFO` & `ezdxf-1.3.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.0rc0
+Version: 1.3.1b0
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.0rc0/pyproject.toml` & `ezdxf-1.3.1b0/pyproject.toml`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/README.md` & `ezdxf-1.3.1b0/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/setup.py` & `ezdxf-1.3.1b0/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_acad_table.py` & `ezdxf-1.3.1b0/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_acis_entites.py` & `ezdxf-1.3.1b0/integration_tests/test_acis_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_appsettings.py` & `ezdxf-1.3.1b0/integration_tests/test_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py` & `ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_document_guid.py` & `ezdxf-1.3.1b0/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py` & `ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py` & `ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py` & `ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_geo.py` & `ezdxf-1.3.1b0/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_groups.py` & `ezdxf-1.3.1b0/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_launcher.py` & `ezdxf-1.3.1b0/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py` & `ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py` & `ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_odafc.py` & `ezdxf-1.3.1b0/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py` & `ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py` & `ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_r12export.py` & `ezdxf-1.3.1b0/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_r12strict.py` & `ezdxf-1.3.1b0/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_r12writer.py` & `ezdxf-1.3.1b0/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_recover.py` & `ezdxf-1.3.1b0/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py` & `ezdxf-1.3.1b0/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py` & `ezdxf-1.3.1b0/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py` & `ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py` & `ezdxf-1.3.1b0/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/test_xref_load_acis.py` & `ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip` & `ezdxf-1.3.1b0/integration_tests/data/dynblks.zip`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf` & `ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/groups.dxf` & `ezdxf-1.3.1b0/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf` & `ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf` & `ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf` & `ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf` & `ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf` & `ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf` & `ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf` & `ezdxf-1.3.1b0/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf` & `ezdxf-1.3.1b0/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf` & `ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf` & `ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/appsettings.py` & `ezdxf-1.3.1b0/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/audit.py` & `ezdxf-1.3.1b0/src/ezdxf/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     REMOVED_UNSUPPORTED_SECTION = 9
     REMOVED_UNSUPPORTED_TABLE = 10
     REMOVED_INVALID_GRAPHIC_ENTITY = 11
     REMOVED_INVALID_DXF_OBJECT = 12
     REMOVED_STANDALONE_ATTRIB_ENTITY = 13
     MISPLACED_ROOT_DICT = 14
     ROOT_DICT_NOT_FOUND = 15
+    REMOVED_ENTITY_WITH_INVALID_OWNER_HANDLE = 16
 
     UNDEFINED_LINETYPE = 100
     UNDEFINED_DIMENSION_STYLE = 101
     UNDEFINED_TEXT_STYLE = 102
     UNDEFINED_BLOCK = 103
     INVALID_BLOCK_REFERENCE_CYCLE = 104
     REMOVE_EMPTY_GROUP = 105
@@ -85,14 +86,15 @@
     INVALID_SPLINE_FIT_POINT_COUNT = 219
     INVALID_SPLINE_KNOT_VALUE_COUNT = 220
     INVALID_SPLINE_WEIGHT_COUNT = 221
     INVALID_DIMENSION_GEOMETRY_LOCATION = 222
     INVALID_TRANSPARENCY = 223
     INVALID_CREASE_VALUE_COUNT = 224
     INVALID_ELLIPSE_RATIO = 225
+    INVALID_HATCH_BOUNDARY_PATH = 226
 
 
 REQUIRED_ROOT_DICT_ENTRIES = ("ACAD_GROUP", "ACAD_PLOTSTYLENAME")
 
 
 class ErrorEntry:
     def __init__(
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/bbox.py` & `ezdxf-1.3.1b0/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py` & `ezdxf-1.3.1b0/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/colors.py` & `ezdxf-1.3.1b0/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/commands.py` & `ezdxf-1.3.1b0/src/ezdxf/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/comments.py` & `ezdxf-1.3.1b0/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/disassemble.py` & `ezdxf-1.3.1b0/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/document.py` & `ezdxf-1.3.1b0/src/ezdxf/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,27 +48,27 @@
 from ezdxf.lldxf.tagwriter import (
     AbstractTagWriter,
     TagWriter,
     BinaryTagWriter,
     JSONTagWriter,
 )
 from ezdxf.query import EntityQuery
-from ezdxf.protocols import SupportsTemporaryTransformation
 from ezdxf.render.dimension import DimensionRenderer
 from ezdxf.sections.acdsdata import AcDsDataSection, new_acds_data_section
 from ezdxf.sections.blocks import BlocksSection
 from ezdxf.sections.classes import ClassesSection
 from ezdxf.sections.entities import EntitySection, StoredSection
 from ezdxf.sections.header import HeaderSection
 from ezdxf.sections.objects import ObjectsSection
 from ezdxf.sections.tables import TablesSection
 from ezdxf.tools import guid
 from ezdxf.tools.codepage import tocodepage, toencoding
 from ezdxf.tools.juliandate import juliandate
 from ezdxf.tools.text import safe_string, MAX_STR_LEN
+from ezdxf import messenger, msgtypes
 
 
 logger = logging.getLogger("ezdxf")
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFEntity, Layer, VPort, Dictionary
     from ezdxf.eztypes import GenericLayoutType
@@ -107,14 +107,15 @@
         seed = START_HANDLE
     return seed
 
 
 class Drawing:
     def __init__(self, dxfversion=DXF2013) -> None:
         self.entitydb = EntityDB()
+        self.messenger = messenger.Messenger(self)
         target_dxfversion = dxfversion.upper()
         self._dxfversion: str = const.acad_release_to_dxf_version.get(
             target_dxfversion, target_dxfversion
         )
         if self._dxfversion not in const.versions_supported_by_new:
             raise const.DXFVersionError(f'Unsupported DXF version "{self.dxfversion}".')
         # Store original dxf version if loaded (and maybe converted R13/14)
@@ -582,16 +583,16 @@
             binary = doc.encode(stream.get_value())
 
         Args:
             stream: output text stream or binary stream
             fmt: "asc" for ASCII DXF (default) or "bin" for binary DXF
 
         """
-        # These changes may alter the document content (create new entities, blocks ...) 
-        # and have to be done before the export and the update of internal structures 
+        # These changes may alter the document content (create new entities, blocks ...)
+        # and have to be done before the export and the update of internal structures
         # can be done.
         self.commit_pending_changes()
 
         dxfversion = self.dxfversion
         if dxfversion == DXF12:
             handles = bool(self.header.get("$HANDLING", 0))
         else:
@@ -643,17 +644,15 @@
             self.acdsdata.export_dxf(tagwriter)
         for section in self.stored_sections:
             section.export_dxf(tagwriter)
 
         tagwriter.write_tag2(0, "EOF")
 
     def commit_pending_changes(self) -> None:
-        entities = list(self.entitydb.values())  # entitydb may change while iterating
-        for entity in entities:
-            entity.commit_pending_changes()
+        self.messenger.broadcast(msgtypes.COMMIT_PENDING_CHANGES)
 
     def update_all(self) -> None:
         if self.dxfversion > DXF12:
             self.classes.add_required_classes(self.dxfversion)
         self._create_appids()
         self._update_header_vars()
         self.update_extents()
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py` & `ezdxf-1.3.1b0/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py` & `ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entitydb.py` & `ezdxf-1.3.1b0/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/enums.py` & `ezdxf-1.3.1b0/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/explode.py` & `ezdxf-1.3.1b0/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/eztypes.py` & `ezdxf-1.3.1b0/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py` & `ezdxf-1.3.1b0/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py` & `ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py` & `ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,28 @@
     global_bspline_interpolation,
     fit_points_to_cad_cv,
     arc_angle_span_deg,
     ConstructionArc,
     NULLVEC,
 )
 from ezdxf.render.arrows import ARROWS
-from ezdxf.entities import factory, Point, Spline, Body, Surface, Line
+from ezdxf.entities import factory, Point, Spline, Body, Surface, Line, Circle
 from ezdxf.entities.mtext_columns import *
 from ezdxf.entities.dimstyleoverride import DimStyleOverride
 from ezdxf.render.dim_linear import multi_point_linear_dimension
 from ezdxf.tools import guid
 
 logger = logging.getLogger("ezdxf")
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.eztypes import GenericLayoutType
     from ezdxf.entities import (
         Arc,
         AttDef,
-        Circle,
         Dimension,
         ArcDimension,
         DXFGraphic,
         Ellipse,
         ExtrudedSurface,
         Face3d,
         Hatch,
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/groupby.py` & `ezdxf-1.3.1b0/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/npshapes.py` & `ezdxf-1.3.1b0/src/ezdxf/npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/protocols.py` & `ezdxf-1.3.1b0/src/ezdxf/protocols.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  Copyright (c) 2021-2024, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterator, Iterable
+from typing import TYPE_CHECKING, Iterator, Iterable, Any
 from typing_extensions import Protocol, runtime_checkable
 from ezdxf.query import EntityQuery
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFGraphic, DXFEntity
     from ezdxf.entities.temporary_transform import TemporaryTransformation
     from ezdxf.math import Matrix44, AbstractBoundingBox
@@ -85,7 +85,12 @@
 class SupportsBoundingBox(Protocol):
     def bbox(self) -> AbstractBoundingBox: ...
 
 
 @runtime_checkable
 class SupportsTemporaryTransformation(Protocol):
     def temporary_transformation(self) -> TemporaryTransformation: ...
+
+
+class SupportsMessages(Protocol):
+    def notify(self, message_type: int, data: Any = None) -> None:
+        """Internal messaging system."""
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py` & `ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/query.py` & `ezdxf-1.3.1b0/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/queryparser.py` & `ezdxf-1.3.1b0/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/r12strict.py` & `ezdxf-1.3.1b0/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/recover.py` & `ezdxf-1.3.1b0/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/reorder.py` & `ezdxf-1.3.1b0/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/revcloud.py` & `ezdxf-1.3.1b0/src/ezdxf/revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/select.py` & `ezdxf-1.3.1b0/src/ezdxf/select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/transform.py` & `ezdxf-1.3.1b0/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/units.py` & `ezdxf-1.3.1b0/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/upright.py` & `ezdxf-1.3.1b0/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/urecord.py` & `ezdxf-1.3.1b0/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/version.py` & `ezdxf-1.3.1b0/src/ezdxf/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 3, 0, "rc0")
-__version__ = "1.3.0rc0"
+version = (1, 3, 1, "b0")
+__version__ = "1.3.1b0"
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/xclip.py` & `ezdxf-1.3.1b0/src/ezdxf/xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/xref.py` & `ezdxf-1.3.1b0/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/zoom.py` & `ezdxf-1.3.1b0/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/_options.py` & `ezdxf-1.3.1b0/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/__main__.py` & `ezdxf-1.3.1b0/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd` & `ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx` & `ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/api.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#  Copyright (c) 2022-2024, Manfred Moitzi
-#  License: MIT License
+# Copyright (c) 2022-2024, Manfred Moitzi
+# License: MIT License
 # Public API module (interface)
 """
 The main goals of this ACIS support library is:
 
     1. load and parse simple and known ACIS data structures
     2. create and export simple and known ACIS data structures
 
@@ -20,11 +20,12 @@
 """
 from .const import (
     AcisException,
     ParsingError,
     InvalidLinkStructure,
     ExportError,
 )
-from .mesh import mesh_from_body, body_from_mesh
+from .mesh import mesh_from_body, body_from_mesh, vertices_from_body
 from .entities import load, export_sat, export_sab, Body
 from .dbg import AcisDebugger, dump_sab_as_text
-from .dxf import export_dxf, load_dxf
+from .dxf import export_dxf, load_dxf
+from .cache import AcisCache
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/const.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #  Copyright (c) 2022-2024, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import Union, Callable, Type, Any, Sequence, Iterator
+from typing import Callable, Type, Any, Sequence, Iterator
 import abc
 
 from . import sab, sat, const, hdr
 from .const import Features
 from .abstract import DataLoader, AbstractEntity, DataExporter
+from .type_hints import EncodedData
 from ezdxf.math import Matrix44, Vec3, NULLVEC
 
 Factory = Callable[[AbstractEntity], "AcisEntity"]
 
 ENTITY_TYPES: dict[str, Type[AcisEntity]] = {}
 INF = float("inf")
 
 
-def load(data: Union[str, Sequence[str], bytes, bytearray]) -> list[Body]:
+def load(data: EncodedData) -> list[Body]:
     """Returns a list of :class:`Body` entities from :term:`SAT` or :term:`SAB`
     data. Accepts :term:`SAT` data as a single string or a sequence of strings
     and :term:`SAB` data as bytes or bytearray.
 
     """
     if isinstance(data, (bytes, bytearray)):
         return SabLoader.load(data)
@@ -729,15 +730,15 @@
         self.location = Vec3(loader.read_vec3())
 
     def write_data(self, exporter: DataExporter) -> None:
         exporter.write_loc_vec3(self.location)
 
 
 class FileLoader(abc.ABC):
-    records: Sequence[Union[sat.SatEntity, sab.SabEntity]]
+    records: Sequence[sat.SatEntity | sab.SabEntity]
 
     def __init__(self, version: int):
         self.entities: dict[int, AcisEntity] = {}
         self.version: int = version
 
     def entity_factory(self, raw_entity: AbstractEntity) -> AcisEntity:
         uid = id(raw_entity)
@@ -766,36 +767,36 @@
 
     @abc.abstractmethod
     def make_data_loader(self, data: list[Any]) -> DataLoader:
         pass
 
 
 class SabLoader(FileLoader):
-    def __init__(self, data: Union[bytes, bytearray]):
+    def __init__(self, data: bytes | bytearray):
         builder = sab.parse_sab(data)
         super().__init__(builder.header.version)
         self.records = builder.entities
 
     def make_data_loader(self, data: list[Any]) -> DataLoader:
         return sab.SabDataLoader(data, self.version)
 
     @classmethod
-    def load(cls, data: Union[bytes, bytearray]) -> list[Body]:
+    def load(cls, data: bytes | bytearray) -> list[Body]:
         loader = cls(data)
         loader.load_entities()
         return loader.bodies()
 
 
 class SatLoader(FileLoader):
-    def __init__(self, data: Union[str, Sequence[str]]):
+    def __init__(self, data: str | Sequence[str]):
         builder = sat.parse_sat(data)
         super().__init__(builder.header.version)
         self.records = builder.entities
 
     def make_data_loader(self, data: list[Any]) -> DataLoader:
         return sat.SatDataLoader(data, self.version)
 
     @classmethod
-    def load(cls, data: Union[str, Sequence[str]]) -> list[Body]:
+    def load(cls, data: str | Sequence[str]) -> list[Body]:
         loader = cls(data)
         loader.load_entities()
         return loader.bodies()
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -329,7 +329,87 @@
 def make_vertices(vertices: Iterable[Vec3]) -> Iterator[entities.Vertex]:
     for v in vertices:
         point = entities.Point()
         point.location = v
         vertex = entities.Vertex()
         vertex.point = point
         yield vertex
+
+
+def vertices_from_body(body: Body) -> list[Vec3]:
+    """Returns all stored vertices in the given :class:`Body` entity.
+    The result is not optimized, meaning the vertices are in no particular order and
+    there are duplicates.
+
+    This function can be useful to determining the approximate bounding box of an 
+    :term:`ACIS` entity.  The result is exact for polyhedra with flat faces with 
+    straight edges, but not for bodies with curved edges and faces.
+
+    Args:
+        body: ACIS entity of type :class:`Body`
+
+    Raises:
+        TypeError: given `body` entity has invalid type
+
+    """
+
+    if not isinstance(body, Body):
+        raise TypeError(f"expected a body entity, got: {type(body)}")
+    lump = body.lump
+    transform = body.transform
+    vertices: list[Vec3] = []
+
+    m: Optional[Matrix44] = None
+    if not transform.is_none:
+        m = transform.matrix
+    while not lump.is_none:
+        vertices.extend(vertices_from_lump(lump, m))
+        lump = lump.next_lump
+    return vertices
+
+
+def vertices_from_lump(lump: Lump, m: Matrix44 | None = None) -> list[Vec3]:
+    """Returns all stored vertices from a given :class:`Lump` entity. 
+    Applies the transformation :class:`~ezdxf.math.Matrix44` `m` to all vertices if not 
+    ``None``.
+
+    Args:
+        lump: :class:`Lump` entity
+        m: optional transformation matrix
+
+    Raises:
+        TypeError: `lump` has invalid ACIS type
+
+    """
+    if not isinstance(lump, Lump):
+        raise TypeError(f"expected a lump entity, got: {type(lump)}")
+
+    vertices: list[Vec3] = []
+    shell = lump.shell
+    if shell.is_none:
+        return vertices  # not a shell
+
+    face = shell.face
+    while not face.is_none:
+        first_coedge = NONE_REF
+        try:
+            first_coedge = face.loop.coedge
+        except AttributeError:  # loop is a none-entity
+            pass
+        coedge = first_coedge
+        while not coedge.is_none:  # invalid coedge or face is not closed
+            # the edge entity contains the vertices and the curve type
+            edge = coedge.edge
+            try:
+                vertices.append(edge.start_vertex.point.location)
+                vertices.append(edge.end_vertex.point.location)
+            except AttributeError:
+                # one of the involved entities is a none-entity or an
+                # incompatible entity type -> ignore this face!
+                break
+            coedge = coedge.next_coedge
+            if coedge is first_coedge:  # a valid closed face
+                break
+        face = face.next_face
+    if m is not None:
+        return list(m.transform_vertices(vertices))
+    return vertices
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py` & `ezdxf-1.3.1b0/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,15 +721,15 @@
             nonlocal line_index
             line = lines[line_index]
             if line.endswith("{"):  # start of a list
                 line_index += 1
                 return get_mapping()
             else:  # it's a simple name=value line
                 value: str = line.split("=", 1)[1]
-                value = value.lstrip('"')  # strings look like this: name="value
+                value = sanitized_value(value)
                 line_index += 1
             return value
 
         def skip_empty_lines():
             nonlocal line_index
             while line_index < len(lines) and len(lines[line_index]) == 0:
                 line_index += 1
@@ -741,14 +741,26 @@
             yield name, value
             skip_empty_lines()
 
     def get(self, name: str, default: Any) -> Any:
         return self.data.get(name, default)
 
 
+def sanitized_value(value: str) -> str:
+    value = value.strip()
+    if value.startswith('"'):  # strings: <name>="string
+        return value[1:]
+
+    # remove unknown appendix like this: "0.0076200000000 (+7.Z+"8V?S_LC )"
+    # the pattern is "<float|int> (<some data>)", see issue #1069
+    if value.endswith(")"):
+        return value.split(" ")[0]
+    return value
+
+
 def int2color(color: int) -> tuple[int, int, int, int]:
     """Convert color integer value from CTB-file to ``(r, g, b, color_type)
     tuple.
     """
     # Take color from layer, ignore other bytes.
     color_type = (color & 0xFF000000) >> 24
     red = (color & 0xFF0000) >> 16
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,15 +758,15 @@
 
     def _polygon(self, entity: DXFPolygon):
         add_line = self.add_source_code_line
         if len(entity.seeds):
             add_line(f"e.set_seed_points({entity.seeds})")
         if entity.pattern:
             self.add_list_source_code(
-                entity.pattern.lines,
+                map(str, entity.pattern.lines),
                 prolog="e.set_pattern_definition([",
                 epilog="])",
             )
             self.add_source_code_line("e.dxf.solid_fill = 0")
         arg = "    {}={},"
 
         if entity.gradient is not None:
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,18 @@
         odafc.UnsupportedFileFormat: unsupported file extension
         odafc.ODAFCNotInstalledError: ODA File Converter not installed
 
     """
     infile = Path(filename).absolute()
     if not infile.is_file():
         raise FileNotFoundError(f"No such file: '{infile}'")
-    version = _detect_version(filename) if version is None else version
+    if isinstance(version, str):
+        version = map_version(version)
+    else:
+        version = _detect_version(filename)
 
     with tempfile.TemporaryDirectory(prefix="odafc_") as tmp_dir:
         args = _odafc_arguments(
             infile.name,
             str(infile.parent),
             tmp_dir,
             output_format="DXF",
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,14 @@
         """Implements the SupportsVirtualEntities protocol."""
         from ezdxf.proxygraphic import ProxyGraphic
 
         if self.proxy_graphic:
             for e in ProxyGraphic(self.proxy_graphic, doc=self.doc).virtual_entities():
                 e.set_source_of_copy(self)
                 yield e
-        return []
 
     def virtual_entities(self) -> Iterator[DXFGraphic]:
         """Yields proxy graphic as "virtual" entities."""
         return self.__virtual_entities__()
 
     def explode(self, target_layout: Optional[BaseLayout] = None) -> EntityQuery:
         """Explodes the proxy graphic for the ACAD_PROXY_ENTITY into the target layout,
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,35 +442,36 @@
     If the count of table rows or table columns is missing the complete content is
     stored in the first row.
     """
     if table.dxftype() != "ACAD_TABLE":
         raise const.DXFTypeError(f"Expected ACAD_TABLE entity, got {str(table)}")
     acdb_table = table.xtags.get_subclass("AcDbTable")
 
-    values = [tag.value for tag in acdb_table.find_all(302)]
     nrows = acdb_table.get_first_value(91, 0)
     ncols = acdb_table.get_first_value(92, 0)
-    values = _load_table_values(acdb_table)
+    split_code = 171  # DXF R2004
+    if acdb_table.has_tag(302):
+        split_code = 301  # DXF R2007 and later
+    values = _load_table_values(acdb_table, split_code)
     if nrows * ncols == 0:
         return [values]
     content: list[list[str]] = []
     for index in range(nrows):
         start = index * ncols
         content.append(values[start : start + ncols])
     return content
 
 
-def _load_table_values(tags: Tags) -> list[str]:
+def _load_table_values(tags: Tags, split_code: int) -> list[str]:
     values: list[str] = []
-    for group in group_tags(tags, splitcode=301):
+    for group in group_tags(tags, splitcode=split_code):
         g_tags = Tags(group)
-        if g_tags.has_tag(302):
+        if g_tags.has_tag(302):  # DXF R2007 and later
             # contains all text as one long string, with more than 66000 chars tested
             values.append(g_tags.get_first_value(302))
-        elif g_tags.has_tag(2):
-            # text is divided into chunks (2, 2, 2, ..., 1)
-            s = "".join(t.value for t in g_tags.find_all(2))
-            s += g_tags.get_first_value(1, "")
+        else:  
+            # DXF R2004
+            # Text is divided into chunks (2, 2, 2, ..., 1) or (3, 3, 3, ..., 1)
+            # DXF reference says group code 2, BricsCAD writes group code 3
+            s = "".join(tag.value for tag in g_tags if 1 <= tag.code <= 3)
             values.append(s)
-        else:  # unknown tag structure
-            values.append("")
     return values
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/acis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, Union, Optional, Sequence
-from typing_extensions import Self
+from typing import TYPE_CHECKING, Iterable, Union, Optional, Sequence, Any
+from typing_extensions import Self, override
 import logging
 
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     group_code_mapping,
 )
 from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags, DXFTag
 from ezdxf.math import Matrix44
 from ezdxf.tools import crypt, guid
+from ezdxf import msgtypes
 
 from .dxfentity import base_class, SubclassProcessor
 from .dxfgfx import DXFGraphic, acdb_entity
 from .factory import register_entity
 from .copy import default_copy
 from .temporary_transform import TransformByBlockReference
 
@@ -133,21 +134,23 @@
         ``False`` if the entity contains :term:`SAT` data.
         """
         if self.doc:
             return self.doc.dxfversion >= const.DXF2013
         else:
             return False
 
+    @override
     def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, Body)
         entity.sat = self.sat
         entity.sab = self.sab  # load SAB on demand
         entity.dxf.uid = guid()
         entity._temporary_transformation = self._temporary_transformation
 
+    @override
     def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         super().map_resources(clone, mapping)
         clone.convert_acis_data()
 
     def convert_acis_data(self) -> None:
         if self.doc is None:
@@ -161,17 +164,20 @@
         else:
             if self._sat:
                 self._sat = tuple()
                 msg = "DXF version mismatch, can't convert ACIS data from SAT to SAB, SAT data removed."
         if msg:
             logger.info(msg)
 
-    def commit_pending_changes(self) -> None:
-        self._temporary_transformation.apply_transformation(self)
+    @override
+    def notify(self, message_type: int, data: Any = None) -> None:
+        if message_type == msgtypes.COMMIT_PENDING_CHANGES:
+            self._temporary_transformation.apply_transformation(self)
 
+    @override
     def preprocess_export(self, tagwriter: AbstractTagWriter) -> bool:
         msg = ""
         if tagwriter.dxfversion < const.DXF2013:
             valid = len(self.sat) > 0
             if not valid:
                 msg = f"{str(self)} doesn't have SAT data, skipping DXF export"
         else:
@@ -180,14 +186,15 @@
                 msg = f"{str(self)} doesn't have SAB data, skipping DXF export"
         if not valid:
             logger.info(msg)
         if valid and self._temporary_transformation.get_matrix() is not None:
             logger.warning(f"{str(self)} has unapplied temporary transformations.")
         return valid
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         """Loading interface. (internal API)"""
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
@@ -198,14 +205,15 @@
         return dxf
 
     def load_sat_data(self, tags: Tags):
         """Loading interface. (internal API)"""
         text_lines = tags2textlines(tag for tag in tags if tag.code in (1, 3))
         self._sat = tuple(crypt.decode(text_lines))
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags. (internal API)"""
         super().export_entity(tagwriter)
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_modeler_geometry.name)
         if tagwriter.dxfversion >= const.DXF2013:
             # ACIS data is stored in the ACDSDATA section as SAB
             if self.doc and self._update:
@@ -235,19 +243,21 @@
         SAT data.
         """
         if self.has_binary_data:
             return ""
         else:
             return "\n".join(self.sat)
 
+    @override
     def destroy(self) -> None:
         if self.has_binary_data:
             self.doc.acdsdata.del_acis_data(self.dxf.handle)  # type: ignore
         super().destroy()
 
+    @override
     def transform(self, m: Matrix44) -> Self:
         self._temporary_transformation.add_matrix(m)
         return self
 
     def temporary_transformation(self) -> TransformByBlockReference:
         return self._temporary_transformation
 
@@ -303,22 +313,24 @@
     """DXF 3DSOLID entity - container entity for embedded ACIS data."""
 
     DXFTYPE = "3DSOLID"
     DXFATTRIBS = DXFAttributes(
         base_class, acdb_entity, acdb_modeler_geometry, acdb_3dsolid
     )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(dxf, acdb_3dsolid_group_codes, 3)
         return dxf
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         if tagwriter.dxfversion > const.DXF2004:
@@ -353,22 +365,24 @@
     """DXF SURFACE entity - container entity for embedded ACIS data."""
 
     DXFTYPE = "SURFACE"
     DXFATTRIBS = DXFAttributes(
         base_class, acdb_entity, acdb_modeler_geometry, acdb_surface
     )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(dxf, acdb_surface_group_codes, 3)
         return dxf
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_surface.name)
@@ -423,27 +437,29 @@
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_extruded_entity = Matrix44()
         self.sweep_entity_transformation_matrix = Matrix44()
         self.path_entity_transformation_matrix = Matrix44()
 
+    @override
     def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, ExtrudedSurface)
         super().copy_data(entity, copy_strategy)
         entity.transformation_matrix_extruded_entity = (
             self.transformation_matrix_extruded_entity.copy()
         )
         entity.sweep_entity_transformation_matrix = (
             self.sweep_entity_transformation_matrix.copy()
         )
         entity.path_entity_transformation_matrix = (
             self.path_entity_transformation_matrix.copy()
         )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_extruded_surface_group_codes, 4, log=False
@@ -452,14 +468,15 @@
         return dxf
 
     def load_matrices(self, tags: Tags):
         self.transformation_matrix_extruded_entity = load_matrix(tags, code=40)
         self.sweep_entity_transformation_matrix = load_matrix(tags, code=46)
         self.path_entity_transformation_matrix = load_matrix(tags, code=47)
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_extruded_surface.name)
@@ -536,35 +553,38 @@
         acdb_lofted_surface,
     )
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_lofted_entity = Matrix44()
 
+    @override
     def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, LoftedSurface)
         super().copy_data(entity, copy_strategy)
         entity.transformation_matrix_lofted_entity = (
             self.transformation_matrix_lofted_entity.copy()
         )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_lofted_surface_group_codes, 4, log=False
             )
             self.load_matrices(processor.subclasses[4])
         return dxf
 
     def load_matrices(self, tags: Tags):
         self.transformation_matrix_lofted_entity = load_matrix(tags, code=40)
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_lofted_surface.name)
@@ -608,35 +628,38 @@
         acdb_revolved_surface,
     )
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_revolved_entity = Matrix44()
 
+    @override
     def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, RevolvedSurface)
         super().copy_data(entity, copy_strategy)
         entity.transformation_matrix_revolved_entity = (
             self.transformation_matrix_revolved_entity.copy()
         )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_revolved_surface_group_codes, 4, log=False
             )
             self.load_matrices(processor.subclasses[4])
         return dxf
 
     def load_matrices(self, tags: Tags):
         self.transformation_matrix_revolved_entity = load_matrix(tags, code=42)
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_revolved_surface.name)
@@ -724,14 +747,15 @@
     def __init__(self):
         super().__init__()
         self.transformation_matrix_sweep_entity = Matrix44()
         self.transformation_matrix_path_entity = Matrix44()
         self.sweep_entity_transformation_matrix = Matrix44()
         self.path_entity_transformation_matrix = Matrix44()
 
+    @override
     def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, SweptSurface)
         super().copy_data(entity, copy_strategy)
         entity.transformation_matrix_sweep_entity = (
             self.transformation_matrix_sweep_entity.copy()
         )
         entity.transformation_matrix_path_entity = (
@@ -740,14 +764,15 @@
         entity.sweep_entity_transformation_matrix = (
             self.sweep_entity_transformation_matrix.copy()
         )
         entity.path_entity_transformation_matrix = (
             self.path_entity_transformation_matrix.copy()
         )
 
+    @override
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_swept_surface_group_codes, 4, log=False
@@ -757,14 +782,15 @@
 
     def load_matrices(self, tags: Tags):
         self.transformation_matrix_sweep_entity = load_matrix(tags, code=40)
         self.transformation_matrix_path_entity = load_matrix(tags, code=41)
         self.sweep_entity_transformation_matrix = load_matrix(tags, code=46)
         self.path_entity_transformation_matrix = load_matrix(tags, code=47)
 
+    @override
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
         tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_swept_surface.name)
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/block.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,65 +60,65 @@
 
 class AbstractBoundaryPath(abc.ABC):
     type: BoundaryPathType
     path_type_flags: int
     source_boundary_objects: list[str]
 
     @abc.abstractmethod
-    def clear(self) -> None:
-        ...
+    def clear(self) -> None: ...
 
     @classmethod
     @abc.abstractmethod
-    def load_tags(cls, tags: Tags) -> AbstractBoundaryPath:
-        ...
+    def load_tags(cls, tags: Tags) -> AbstractBoundaryPath: ...
 
     @abc.abstractmethod
-    def export_dxf(self, tagwriter: AbstractTagWriter, dxftype: str) -> None:
-        ...
+    def export_dxf(self, tagwriter: AbstractTagWriter, dxftype: str) -> None: ...
 
     @abc.abstractmethod
-    def transform(self, ocs: OCSTransform, elevation: float) -> None:
-        ...
+    def transform(self, ocs: OCSTransform, elevation: float) -> None: ...
 
+    @abc.abstractmethod
+    def is_valid(self) -> bool: ...
 
 class AbstractEdge(abc.ABC):
     type: EdgeType
 
     @property
     @abc.abstractmethod
-    def start_point(self) -> Vec2:
-        ...
+    def start_point(self) -> Vec2: ...
 
     @property
     @abc.abstractmethod
-    def end_point(self) -> Vec2:
-        ...
+    def end_point(self) -> Vec2: ...
 
     @abc.abstractmethod
-    def export_dxf(self, tagwriter: AbstractTagWriter) -> None:
-        ...
+    def export_dxf(self, tagwriter: AbstractTagWriter) -> None: ...
 
     @abc.abstractmethod
-    def transform(self, ocs: OCSTransform, elevation: float) -> None:
-        ...
+    def transform(self, ocs: OCSTransform, elevation: float) -> None: ...
+
+    @abc.abstractmethod
+    def is_valid(self) -> bool: ...
 
 
 class BoundaryPaths:
     def __init__(self, paths: Optional[list[AbstractBoundaryPath]] = None):
         self.paths: list[AbstractBoundaryPath] = paths or []
 
     def __len__(self):
         return len(self.paths)
 
     def __getitem__(self, item):
         return self.paths[item]
 
     def __iter__(self):
         return iter(self.paths)
+    
+    def is_valid(self) -> bool:
+        return  all(p.is_valid() for p in self.paths)
 
     @classmethod
     def load_tags(cls, tags: Tags) -> BoundaryPaths:
         paths = []
         assert tags[0].code == 92
         grouped_path_tags = group_tags(tags, splitcode=92)
         for path_tags in grouped_path_tags:
@@ -565,14 +565,17 @@
         # list of 2D coordinates with bulge values (x, y, bulge);
         # bulge default = 0.0
         self.vertices: list[tuple[float, float, float]] = []
         # MPOLYGON does not support source boundary objects, the MPOLYGON is
         # the source object!
         self.source_boundary_objects: list[str] = []  # (330, handle) tags
 
+    def is_valid(self) -> bool:
+        return True
+    
     @classmethod
     def from_vertices(
         cls,
         path_vertices: Iterable[tuple[float, ...]],
         is_closed: bool = True,
         flags: int = 1,
     ) -> PolylinePath:
@@ -698,14 +701,17 @@
         self.path_type_flags = const.BOUNDARY_PATH_DEFAULT
         self.edges: list[AbstractEdge] = []
         self.source_boundary_objects = []
 
     def __iter__(self):
         return iter(self.edges)
 
+    def is_valid(self) -> bool:
+        return all(e.is_valid() for e in self.edges)
+
     @classmethod
     def load_tags(cls, tags: Tags) -> EdgePath:
         edge_path = cls()
         edge_path.source_boundary_objects = pop_source_boundary_objects_tags(
             tags
         )
         for edge_tags in group_tags(tags, splitcode=72):
@@ -924,14 +930,17 @@
     EDGE_TYPE = "LineEdge"  # 2021-05-31: deprecated use type
     type = EdgeType.LINE
 
     def __init__(self):
         self.start = Vec2(0, 0)  # OCS!
         self.end = Vec2(0, 0)  # OCS!
 
+    def is_valid(self) -> bool:
+        return True
+    
     @property
     def start_point(self) -> Vec2:
         return self.start
 
     @property
     def end_point(self) -> Vec2:
         return self.end
@@ -972,14 +981,17 @@
         self.radius: float = 1.0
         # Start- and end angles are always stored in counter-clockwise order!
         self.start_angle: float = 0.0
         self.end_angle: float = 360.0
         # Flag to preserve the required orientation for DXF export:
         self.ccw: bool = True
 
+    def is_valid(self) -> bool:
+        return True
+
     @property
     def start_point(self) -> Vec2:
         return self.construction_tool().start_point
 
     @property
     def end_point(self) -> Vec2:
         return self.construction_tool().end_point
@@ -1077,14 +1089,17 @@
         self.ratio: float = 1.0
         # Start- and end angles are always stored in counter-clockwise order!
         self.start_angle: float = 0.0  # start param, not a real angle
         self.end_angle: float = 360.0  # end param, not a real angle
         # Flag to preserve the required orientation for DXF export:
         self.ccw: bool = True
 
+    def is_valid(self) -> bool:
+        return True
+
     @property
     def start_point(self) -> Vec2:
         return self.construction_tool().start_point.vec2
 
     @property
     def end_point(self) -> Vec2:
         return self.construction_tool().end_point.vec2
@@ -1226,14 +1241,27 @@
         self.control_points: list[Vec2] = []
         self.fit_points: list[Vec2] = []
         self.weights: list[float] = []
         # do not set tangents by default to (0, 0)
         self.start_tangent: Optional[Vec2] = None
         self.end_tangent: Optional[Vec2] = None
 
+    def is_valid(self) -> bool:
+        if len(self.control_points):
+            order = self.degree + 1
+            count = len(self.control_points)
+            if order > count:
+                return False
+            required_knot_count = count + order
+            if len(self.knot_values) != required_knot_count:
+                return False
+        elif len(self.fit_points) < 2:
+            return False
+        return True
+
     @property
     def start_point(self) -> Vec2:
         return self.control_points[0]
 
     @property
     def end_point(self) -> Vec2:
         return self.control_points[-1]
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/copy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,19 +616,16 @@
         del self.extension_dict
         del self.appdata
         del self.reactors
         del self.xdata
         del self.doc
         del self.dxf  # check mark for is_alive
 
-    def commit_pending_changes(self) -> None:
-        """Commit all unapplied changes like temporary transformations of ACIS entities.
-
-        (internal API)
-        """
+    def notify(self, message_type: int, data: Any = None) -> None:
+        """Internal messaging system.  (internal API)"""
         pass
 
     def preprocess_export(self, tagwriter: AbstractTagWriter) -> bool:
         """Pre requirement check and pre-processing for export.
 
         Returns ``False``  if entity should not be exported at all.
 
@@ -1081,12 +1078,11 @@
         """Implements the SupportsVirtualEntities protocol."""
         from ezdxf.proxygraphic import ProxyGraphic
 
         if self.proxy_graphic:
             for e in ProxyGraphic(self.proxy_graphic, self.doc).virtual_entities():
                 e.set_source_of_copy(self)
                 yield e
-        return []
 
     def virtual_entities(self) -> Iterator[DXFGraphic]:
         """Yields proxy graphic as "virtual" entities."""
         return self.__virtual_entities__()
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023, Manfred Moitzi
+# Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT-License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Iterable,
     Iterator,
     cast,
@@ -188,49 +188,75 @@
                data.pop()
 
         """
         data = list(self)
         yield data
         self.set_data(data)
 
-    def set_data(self, entities: Iterable[DXFEntity]) -> None:
-        """Set `entities` as new group content, entities should be an iterable
-        :class:`DXFGraphic` or inherited (LINE, CIRCLE, ...).
-        Raises :class:`DXFValueError` if not all entities be on the same layout
-        (modelspace or any paperspace layout but not block)
-
-        """
+    def _validate_entities(self, entities: Iterable[DXFEntity]) -> list[DXFEntity]:
         assert self.doc is not None
         entities = list(entities)
         valid_entities = filter_invalid_entities(entities, self.doc, str(self))
         if len(valid_entities) != len(entities):
             raise const.DXFStructureError("invalid entities found")
         if not all_entities_on_same_layout(valid_entities):
             raise const.DXFStructureError(
                 "All entities have to be in the same layout and are not allowed"
                 " to be in a block layout."
             )
+        return valid_entities
+
+    def set_data(self, entities: Iterable[DXFEntity]) -> None:
+        """Set `entities` as new group content, entities should be an iterable of
+        :class:`DXFGraphic` (LINE, CIRCLE, ...).
+
+        Raises:
+            DXFValueError: not all entities are located on the same layout (modelspace
+                or any paperspace layout but not block)
+
+        """
+        valid_entities = self._validate_entities(entities)
         self.clear()
+        self._add_group_reactor(valid_entities)
         self._data = valid_entities
 
     def extend(self, entities: Iterable[DXFEntity]) -> None:
-        """Add `entities` to :class:`DXFGroup` without immediate verification!
+        """Add `entities` to :class:`DXFGroup`, entities should be an iterable of
+        :class:`DXFGraphic` (LINE, CIRCLE, ...).
 
-        Validation at DXF export may raise a :class:`DXFStructureError`!
+        Raises:
+            DXFValueError: not all entities are located on the same layout (modelspace
+                or any paperspace layout but not block)
 
         """
-        self._data.extend(entities)
+        valid_entities = self._validate_entities(entities)
+        handles = set(self.handles())
+        valid_entities = [e for e in valid_entities if e.dxf.handle not in handles]
+        self._add_group_reactor(valid_entities)
+        self._data.extend(valid_entities)
 
     def clear(self) -> None:
         """Remove all entities from :class:`DXFGroup`, does not delete any
         drawing entities referenced by this group.
 
         """
+        # TODO: remove handle of GROUP entity from reactors of entities #1085
+        self._remove_group_reactor(self._data)
         self._data = []
 
+    def _add_group_reactor(self, entities: list[DXFEntity]) -> None:
+        group_handle = self.dxf.handle
+        for entity in entities:
+            entity.append_reactor_handle(group_handle)
+
+    def _remove_group_reactor(self, entities: list[DXFEntity]) -> None:
+        group_handle = self.dxf.handle
+        for entity in entities:
+            entity.discard_reactor_handle(group_handle)
+
     def audit(self, auditor: Auditor) -> None:
         """Remove invalid entities from :class:`DXFGroup`.
 
         Invalid entities are:
 
         - deleted entities
         - all entities which do not reside in model- or paper space
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/image.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 __all__ = ["PlotSettings", "DXFLayout"]
 
 acdb_plot_settings = DefSubclass(
     "AcDbPlotSettings",
     {
         # acdb_plot_settings is also part of LAYOUT and LAYOUT has a 'name' attribute
         "page_setup_name": DXFAttr(1, default=""),
-        "plot_configuration_file": DXFAttr(2, default="Adobe PDF"),
+
+        # An optional empty string selects the default printer/plotter
+        "plot_configuration_file": DXFAttr(2, default="", optional=True),
         "paper_size": DXFAttr(4, default="A3"),
         "plot_view_name": DXFAttr(6, default=""),
         "left_margin": DXFAttr(40, default=7.5),  # in mm
         "bottom_margin": DXFAttr(41, default=20),  # in mm
         "right_margin": DXFAttr(42, default=7.5),  # in mm
         "top_margin": DXFAttr(43, default=20),  # in mm
         "paper_width": DXFAttr(44, default=420),  # in mm
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/light.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/line.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/material.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/point.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # License: MIT License
 from __future__ import annotations
 from typing import Sequence, Optional, Union, TYPE_CHECKING, Iterator
 from typing_extensions import Self
 import abc
 import copy
 
+from ezdxf.audit import Auditor, AuditError
 from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags
 from ezdxf import colors
 from ezdxf.tools import pattern
 from ezdxf.math import Vec3, Matrix44
 from ezdxf.math.transformtools import OCSTransform
 from .boundary_paths import BoundaryPaths
@@ -445,7 +446,18 @@
                 yield from hatching.hatch_entity(self)
             except hatching.HatchingError:
                 return
 
     @abc.abstractmethod
     def set_solid_fill(self, color: int = 7, style: int = 1, rgb: Optional[RGB] = None):
         ...
+    
+    def audit(self, auditor: Auditor) -> None:
+        super().audit(auditor)
+        if not self.is_alive:
+            return
+        if not self.paths.is_valid():
+            auditor.fixed_error(
+                code=AuditError.INVALID_HATCH_BOUNDARY_PATH,
+                message=f"Deleted entity {str(self)} containing invalid boundary paths."
+            )
+            auditor.trash(self)
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/table.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/temporary_transform.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/text.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/view.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py` & `ezdxf-1.3.1b0/src/ezdxf/layouts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,23 @@
         if block_record.has_extension_dict:
             return block_record.get_extension_dict()
         else:
             return block_record.new_extension_dict()
 
     def add_entity(self, entity: DXFGraphic) -> None:
         """Add an existing :class:`DXFGraphic` entity to a layout, but be sure
-        to unlink (:meth:`~BaseLayout.unlink_entity`) entity from the previous
-        owner layout. Adding entities from a different DXF drawing is not
+        to unlink (:meth:`~BaseLayout.unlink_entity`) `entity` from the previous
+        owner layout.  Adding entities from a different DXF drawing is not
         supported.
+
+        .. warning:: 
+        
+            This is a low-level tool - use it with caution and make sure you understand 
+            what you are doing! If used improperly, the DXF document may be damaged.
+
         """
         # bind virtual entities to the DXF document:
         doc = self.doc
         if entity.dxf.handle is None and doc:
             factory.bind(entity, doc)
         handle = entity.dxf.handle
         if handle is None or handle not in self.doc.entitydb:
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py` & `ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py` & `ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py` & `ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/arc.py` & `ezdxf-1.3.1b0/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py` & `ezdxf-1.3.1b0/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py` & `ezdxf-1.3.1b0/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/box.py` & `ezdxf-1.3.1b0/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py` & `ezdxf-1.3.1b0/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py` & `ezdxf-1.3.1b0/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/circle.py` & `ezdxf-1.3.1b0/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py` & `ezdxf-1.3.1b0/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py` & `ezdxf-1.3.1b0/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py` & `ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py` & `ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py` & `ezdxf-1.3.1b0/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py` & `ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py` & `ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py` & `ezdxf-1.3.1b0/src/ezdxf/math/legacy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py` & `ezdxf-1.3.1b0/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/line.py` & `ezdxf-1.3.1b0/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py` & `ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py` & `ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py` & `ezdxf-1.3.1b0/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py` & `ezdxf-1.3.1b0/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py` & `ezdxf-1.3.1b0/src/ezdxf/math/rtree.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,145 +5,141 @@
 # - SsTree JavaScript source code:
 #   (c) 2019, Marcello La Rocca, released under the GNU Affero General Public License v3.0
 #   https://github.com/mlarocca/AlgorithmsAndDataStructuresInAction/tree/master/JavaScript/src/ss_tree
 # - Research paper of Antonin Guttman:
 #   http://www-db.deis.unibo.it/courses/SI-LS/papers/Gut84.pdf
 from __future__ import annotations
 import statistics
-from typing import Iterator, Callable, Sequence, Iterable
+from typing import Iterator, Callable, Sequence, Iterable, TypeVar, Generic
 import abc
 import math
 
-from ezdxf.math import BoundingBox, AnyVec, Vec3, spherical_envelope
+from ezdxf.math import BoundingBox, Vec2, Vec3, spherical_envelope
 
 __all__ = ["RTree"]
 
 INF = float("inf")
 
+T = TypeVar("T", Vec2, Vec3)
 
-class Node(abc.ABC):
+
+class Node(abc.ABC, Generic[T]):
     __slots__ = ("bbox",)
 
     def __init__(self, bbox: BoundingBox):
         self.bbox: BoundingBox = bbox
 
     @abc.abstractmethod
-    def __len__(self) -> int:
-        ...
+    def __len__(self) -> int: ...
 
     @abc.abstractmethod
-    def __iter__(self) -> Iterator[AnyVec]:
-        ...
+    def __iter__(self) -> Iterator[T]: ...
 
     @abc.abstractmethod
-    def contains(self, point: AnyVec) -> bool:
-        ...
+    def contains(self, point: T) -> bool: ...
 
     @abc.abstractmethod
     def _nearest_neighbor(
-        self, target: AnyVec, nn: AnyVec = None, nn_dist: float = INF
-    ) -> tuple[AnyVec, float]:
-        ...
+        self, target: T, nn: T = None, nn_dist: float = INF
+    ) -> tuple[T, float]: ...
 
     @abc.abstractmethod
-    def points_in_sphere(self, center: AnyVec, radius: float) -> Iterator[AnyVec]:
-        ...
+    def points_in_sphere(self, center: T, radius: float) -> Iterator[T]: ...
 
     @abc.abstractmethod
-    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[AnyVec]:
-        ...
+    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[T]: ...
 
-    def nearest_neighbor(self, target: AnyVec) -> tuple[AnyVec, float]:
+    def nearest_neighbor(self, target: T) -> tuple[T, float]:
         return self._nearest_neighbor(target)
 
 
-class LeafNode(Node):
+class LeafNode(Node[T]):
     __slots__ = ("points", "bbox")
 
-    def __init__(self, points: list[AnyVec]):
+    def __init__(self, points: list[T]):
         self.points = tuple(points)
         super().__init__(BoundingBox(self.points))
 
     def __len__(self):
         return len(self.points)
 
-    def __iter__(self) -> Iterator[AnyVec]:
+    def __iter__(self) -> Iterator[T]:
         return iter(self.points)
 
-    def contains(self, point: AnyVec) -> bool:
+    def contains(self, point: T) -> bool:
         return any(point.isclose(p) for p in self.points)
 
     def _nearest_neighbor(
-        self, target: AnyVec, nn: AnyVec = None, nn_dist: float = INF
-    ) -> tuple[AnyVec, float]:
+        self, target: T, nn: T = None, nn_dist: float = INF
+    ) -> tuple[T, float]:
         distance, point = min((target.distance(p), p) for p in self.points)
         if distance < nn_dist:
             nn, nn_dist = point, distance
         return nn, nn_dist
 
-    def points_in_sphere(self, center: AnyVec, radius: float) -> Iterator[AnyVec]:
+    def points_in_sphere(self, center: T, radius: float) -> Iterator[T]:
         return (p for p in self.points if center.distance(p) <= radius)
 
-    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[AnyVec]:
+    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[T]:
         return (p for p in self.points if bbox.inside(p))
 
 
-class InnerNode(Node):
+class InnerNode(Node[T]):
     __slots__ = ("children", "bbox")
 
-    def __init__(self, children: Sequence[Node]):
+    def __init__(self, children: Sequence[Node[T]]):
         super().__init__(BoundingBox())
         self.children = tuple(children)
         for child in self.children:
             # build union of all child bounding boxes
             self.bbox.extend([child.bbox.extmin, child.bbox.extmax])
 
     def __len__(self) -> int:
         return sum(len(c) for c in self.children)
 
-    def __iter__(self) -> Iterator[AnyVec]:
+    def __iter__(self) -> Iterator[T]:
         for child in self.children:
             yield from iter(child)
 
-    def contains(self, point: AnyVec) -> bool:
+    def contains(self, point: T) -> bool:
         for child in self.children:
             if child.bbox.inside(point) and child.contains(point):
                 return True
         return False
 
     def _nearest_neighbor(
-        self, target: AnyVec, nn: AnyVec = None, nn_dist: float = INF
-    ) -> tuple[AnyVec, float]:
+        self, target: T, nn: T = None, nn_dist: float = INF
+    ) -> tuple[T, float]:
         closest_child = find_closest_child(self.children, target)
         nn, nn_dist = closest_child._nearest_neighbor(target, nn, nn_dist)
         for child in self.children:
             if child is closest_child:
                 continue
             # is target inside the child bounding box + nn_dist in all directions
             if grow_box(child.bbox, nn_dist).inside(target):
                 point, distance = child._nearest_neighbor(target, nn, nn_dist)
                 if distance < nn_dist:
                     nn = point
                     nn_dist = distance
         return nn, nn_dist
 
-    def points_in_sphere(self, center: AnyVec, radius: float) -> Iterator[AnyVec]:
+    def points_in_sphere(self, center: T, radius: float) -> Iterator[T]:
         for child in self.children:
             if is_sphere_intersecting_bbox(
                 Vec3(center), radius, child.bbox.center, child.bbox.size
             ):
                 yield from child.points_in_sphere(center, radius)
 
-    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[AnyVec]:
+    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[T]:
         for child in self.children:
             if bbox.has_overlap(child.bbox):
                 yield from child.points_in_bbox(bbox)
 
 
-class RTree:
+class RTree(Generic[T]):
     """Immutable spatial search tree loosely based on `R-trees`_.
 
     The search tree is buildup once at initialization and immutable afterwards,
     because rebuilding the tree after inserting or deleting nodes is very costly
     and also keeps the implementation very simple. Without the ability to
     alter the content the restrictions which forces the tree balance at growing
     and shrinking of the original `R-trees`_, could be ignored, like the fixed
@@ -165,49 +161,49 @@
 
     .. _R-trees: https://en.wikipedia.org/wiki/R-tree
 
     """
 
     __slots__ = ("_root",)
 
-    def __init__(self, points: Iterable[AnyVec], max_node_size: int = 5):
+    def __init__(self, points: Iterable[T], max_node_size: int = 5):
         if max_node_size < 2:
             raise ValueError("max node size must be > 1")
         _points = list(points)
         if len(_points) == 0:
             raise ValueError("no points given")
         self._root = make_node(_points, max_node_size, box_split)
 
     def __len__(self):
         """Returns the count of points in the search tree."""
         return len(self._root)
 
-    def __iter__(self) -> Iterator[AnyVec]:
+    def __iter__(self) -> Iterator[T]:
         """Yields all points in the search tree."""
         yield from iter(self._root)
 
-    def contains(self, point: AnyVec) -> bool:
+    def contains(self, point: T) -> bool:
         """Returns ``True`` if `point` exists, the comparison is done by the
         :meth:`isclose` method and not by the identity operator ``is``.
         """
         return self._root.contains(point)
 
-    def nearest_neighbor(self, target: AnyVec) -> tuple[AnyVec, float]:
+    def nearest_neighbor(self, target: T) -> tuple[T, float]:
         """Returns the closest point to the `target` point and the distance
         between these points.
         """
         return self._root.nearest_neighbor(target)
 
-    def points_in_sphere(self, center: AnyVec, radius: float) -> Iterator[AnyVec]:
+    def points_in_sphere(self, center: T, radius: float) -> Iterator[T]:
         """Returns all points in the range of the given sphere including the
         points at the boundary.
         """
         return self._root.points_in_sphere(center, radius)
 
-    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[AnyVec]:
+    def points_in_bbox(self, bbox: BoundingBox) -> Iterator[T]:
         """Returns all points in the range of the given bounding box including
         the points at the boundary.
         """
         return self._root.points_in_bbox(bbox)
 
     def avg_leaf_size(self, spread: float = 1.0) -> float:
         """Returns the average size of the leaf bounding boxes.
@@ -245,25 +241,25 @@
         distances: list[float] = []
         for leaf in collect_leafs(self._root):
             distances.extend(nearest_neighbor_distances(leaf.points))
         return average_exclusive_outliers(distances, spread)
 
 
 def make_node(
-    points: list[AnyVec],
+    points: list[T],
     max_size: int,
-    split_strategy: Callable[[list[AnyVec], int], Sequence[Node]],
-) -> Node:
+    split_strategy: Callable[[list[T], int], Sequence[Node]],
+) -> Node[T]:
     if len(points) > max_size:
         return InnerNode(split_strategy(points, max_size))
     else:
         return LeafNode(points)
 
 
-def box_split(points: list[AnyVec], max_size: int) -> Sequence[Node]:
+def box_split(points: list[T], max_size: int) -> Sequence[Node[T]]:
     n = len(points)
     size: tuple[float, float, float] = BoundingBox(points).size.xyz
     dim = size.index(max(size))
     points.sort(key=lambda vec: vec[dim])
     k = math.ceil(n / max_size)
     return tuple(
         make_node(points[i : i + k], max_size, box_split) for i in range(0, n, k)
@@ -281,18 +277,20 @@
     if abs(distance.y) > intersection_distance.y:
         return False
     if abs(distance.z) > intersection_distance.z:
         return False
     return True
 
 
-def find_closest_child(children: Sequence[Node], point: AnyVec) -> Node:
+def find_closest_child(children: Sequence[Node[T]], point: T) -> Node[T]:
+    def distance(child: Node) -> float:
+        return point.distance(child.bbox.center)
+
     assert len(children) > 0
-    _, node = min((point.distance(child.bbox.center), child) for child in children)
-    return node
+    return min(children, key=distance)
 
 
 def grow_box(box: BoundingBox, dist: float) -> BoundingBox:
     bbox = box.copy()
     bbox.grow(dist)
     return bbox
 
@@ -305,24 +303,24 @@
     max_value = mean + stdev * spread
     values = [value for value in values if value <= max_value]
     if len(values):
         return sum(values) / len(values)
     return 0.0
 
 
-def collect_leafs(node: Node) -> Iterable[LeafNode]:
+def collect_leafs(node: Node[T]) -> Iterable[LeafNode[T]]:
     """Yields all leaf nodes below the given node."""
     if isinstance(node, LeafNode):
         yield node
     elif isinstance(node, InnerNode):
         for child in node.children:
             yield from collect_leafs(child)
 
 
-def nearest_neighbor_distances(points: Sequence[AnyVec]) -> list[float]:
+def nearest_neighbor_distances(points: Sequence[T]) -> list[float]:
     """Brute force calculation of nearest neighbor distances with a
     complexity of O(n!).
     """
     return [
         min(point.distance(p) for p in points[index + 1 :])
         for index, point in enumerate(points[:-1])
     ]
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/shape.py` & `ezdxf-1.3.1b0/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py` & `ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py` & `ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py` & `ezdxf-1.3.1b0/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py` & `ezdxf-1.3.1b0/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/commands.py` & `ezdxf-1.3.1b0/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/converter.py` & `ezdxf-1.3.1b0/src/ezdxf/path/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     Optional,
     Callable,
     Type,
     TypeVar,
 )
 from typing_extensions import TypeAlias
 from functools import singledispatch, partial
+import logging
+
 from ezdxf.math import (
     ABS_TOL,
     Vec2,
     Vec3,
     NULLVEC,
     Z_AXIS,
     OCS,
@@ -81,14 +83,15 @@
 ]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
 TPolygon = TypeVar("TPolygon", Hatch, MPolygon)
 BoundaryFactory = Callable[[BoundaryPaths, Path, int], None]
+logger = logging.getLogger("ezdxf")
 
 
 @singledispatch
 def make_path(entity, segments: int = 1, level: int = 4) -> Path:
     """Factory function to create a single :class:`Path` object from a DXF
     entity.
 
@@ -242,18 +245,23 @@
 @make_path.register(Hatch)
 def _from_hatch(hatch: Hatch, **kwargs) -> Path:
     ocs = hatch.ocs()
     elevation = hatch.dxf.elevation.z
     offset = NULLVEC
     if isinstance(hatch, MPolygon):
         offset = hatch.dxf.get("offset_vector", NULLVEC)
-    paths = [
-        from_hatch_boundary_path(boundary, ocs, elevation, offset=offset)
-        for boundary in hatch.paths
-    ]
+    try:
+        paths = [
+            from_hatch_boundary_path(boundary, ocs, elevation, offset=offset)
+            for boundary in hatch.paths
+        ]
+    except const.DXFStructureError:  
+        # TODO: fix problems beforehand in audit process? see issue #1081
+        logger.warning(f"invalid data in {str(hatch)}")
+        return Path()
     # looses the boundary path state:
     return tools.to_multi_path(paths)
 
 
 def from_hatch(hatch: DXFPolygon, offset: Vec3 = NULLVEC) -> Iterator[Path]:
     """Yield all HATCH/MPOLYGON boundary paths as separated :class:`Path` objects in WCS
     coordinates.
@@ -521,15 +529,15 @@
 
     """
     if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
-        return []
+        return
     extrusion = Vec3(extrusion)
     reference_point = Vec3(paths[0].start)
     dxfattribs = dict(dxfattribs or {})
     if not Z_AXIS.isclose(extrusion):
         ocs, elevation = _get_ocs(extrusion, reference_point)
         paths = tools.transform_paths_to_ocs(paths, ocs)
         dxfattribs["elevation"] = elevation
@@ -577,15 +585,15 @@
 
     """
     if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
-        return []
+        return
     extrusion = Vec3(extrusion)
     reference_point = Vec3(paths[0].start)
     dxfattribs = dict(dxfattribs or {})
     if not Z_AXIS.isclose(extrusion):
         ocs, elevation = _get_ocs(extrusion, reference_point)
         paths = tools.transform_paths_to_ocs(paths, ocs)
         dxfattribs["elevation"] = Vec3(0, 0, elevation)
@@ -641,17 +649,15 @@
         )
     else:
         # noinspection PyTypeChecker
         boundary_factory = partial(
             build_poly_path, distance=distance, segments=segments
         )
 
-    yield from _polygon_converter(
-        Hatch, paths, boundary_factory, extrusion, dxfattribs
-    )
+    yield from _polygon_converter(Hatch, paths, boundary_factory, extrusion, dxfattribs)
 
 
 def to_mpolygons(
     paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
@@ -740,15 +746,15 @@
     dxfattribs=None,
 ) -> Iterator[TPolygon]:
     if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
-        return []
+        return
 
     extrusion = Vec3(extrusion)
     reference_point = paths[0].start
     _dxfattribs: dict = dict(dxfattribs or {})
     if not Z_AXIS.isclose(extrusion):
         ocs, elevation = _get_ocs(extrusion, reference_point)
         paths = tools.transform_paths_to_ocs(paths, ocs)
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py` & `ezdxf-1.3.1b0/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/path.py` & `ezdxf-1.3.1b0/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py` & `ezdxf-1.3.1b0/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/path/tools.py` & `ezdxf-1.3.1b0/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py` & `ezdxf-1.3.1b0/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/curves.py` & `ezdxf-1.3.1b0/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py` & `ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/forms.py` & `ezdxf-1.3.1b0/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py` & `ezdxf-1.3.1b0/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/leader.py` & `ezdxf-1.3.1b0/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py` & `ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py` & `ezdxf-1.3.1b0/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py` & `ezdxf-1.3.1b0/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/mline.py` & `ezdxf-1.3.1b0/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/point.py` & `ezdxf-1.3.1b0/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py` & `ezdxf-1.3.1b0/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py` & `ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/trace.py` & `ezdxf-1.3.1b0/src/ezdxf/render/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,19 @@
     ParallelRaysError,
     bulge_to_arc,
     ConstructionArc,
 )
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
-    from ezdxf.entities import (
-        DXFGraphic,
-        Solid,
-        Trace,
-        Face3d,
-        LWPolyline,
-        Polyline
-    )
+    from ezdxf.entities import DXFGraphic, Solid, Trace, Face3d, LWPolyline, Polyline
 
 __all__ = ["TraceBuilder", "LinearTrace", "CurvedTrace"]
 
-LinearStation = namedtuple(
-    "LinearStation", ("vertex", "start_width", "end_width")
-)
+LinearStation = namedtuple("LinearStation", ("vertex", "start_width", "end_width"))
 # start_width of the next (following) segment
 # end_width of the next (following) segment
 
 CurveStation = namedtuple("CurveStation", ("vertex0", "vertex1"))
 
 Face: TypeAlias = Tuple[Vec2, Vec2, Vec2, Vec2]
 Polygon: TypeAlias = Sequence[Vec2]
@@ -162,22 +153,18 @@
 
         """
         if end_width is None:
             end_width = start_width
         point = Vec2(point)
         stations = self._stations
 
-        if bool(stations) and stations[-1].vertex.isclose(
-            point, abs_tol=self.abs_tol
-        ):
+        if bool(stations) and stations[-1].vertex.isclose(point, abs_tol=self.abs_tol):
             # replace last station
             stations.pop()
-        stations.append(
-            LinearStation(point, float(start_width), float(end_width))
-        )
+        stations.append(LinearStation(point, float(start_width), float(end_width)))
 
     def faces(self) -> Iterable[Face]:
         """Yields all faces as 4-tuples of :class:`~ezdxf.math.Vec2` objects.
 
         First and last miter is 90 degrees if the path is not closed, otherwise
         the intersection of first and last segment is taken into account,
         a closed path has to have explicit the same last and first vertex.
@@ -207,15 +194,16 @@
             return ray(left1, left2), ray(right1, right2)
 
         def intersect(
             ray1: ConstructionRay, ray2: ConstructionRay, default: Vec2
         ) -> Vec2:
             """Intersect two rays but take parallel rays into account."""
             # check for nearly parallel rays pi/100 ~1.8 degrees
-            if ray1.direction.angle_between(ray2.direction) < 0.031415:
+            angle = abs(ray1.direction.angle_between(ray2.direction))
+            if angle < 0.031415 or abs(math.pi - angle) < 0.031415:
                 return default
             try:
                 return ray1.intersect(ray2)
             except ParallelRaysError:
                 return default
 
         # Path has to be explicit closed by vertices:
@@ -230,17 +218,15 @@
         # 4th vertex right of line at the end, distance = end_width/2
         for station in range(count - 1):
             start_vertex, start_width, end_width = stations[station]
             end_vertex = stations[station + 1].vertex
             # Start- and end vertex are never to close together, close stations
             # will be merged in method LinearTrace.add_station().
             segments.append(
-                _normal_offset_points(
-                    start_vertex, end_vertex, start_width, end_width
-                )
+                _normal_offset_points(start_vertex, end_vertex, start_width, end_width)
             )
 
         # offset rays:
         # 1 is the upper or left of line
         # 2 is the lower or right of line
         offset_ray1, offset_ray2 = offset_rays(0)
         prev_offset_ray1 = None
@@ -252,17 +238,15 @@
         for i in range(len(segments)):
             up1, up2, down1, down2 = segments[i]
             if i == 0:
                 # Set first vertices of the first face.
                 if is_closed:
                     # Compute first two vertices as intersection of first and
                     # last segment
-                    last_offset_ray1, last_offset_ray2 = offset_rays(
-                        len(segments) - 1
-                    )
+                    last_offset_ray1, last_offset_ray2 = offset_rays(len(segments) - 1)
                     vtx0 = intersect(last_offset_ray1, offset_ray1, up1)
                     vtx1 = intersect(last_offset_ray2, offset_ray2, down1)
 
                     # Store last vertices for the closing face.
                     last_up2 = vtx0
                     last_down2 = vtx1
                 else:
@@ -346,15 +330,15 @@
             end_width: end width
             segments: count of segments for approximation
 
         """
         curve_trace = cls()
         count = segments + 1
         t = np.linspace(0, spline.max_t, count)
-        for ((point, derivative), width) in zip(
+        for (point, derivative), width in zip(
             spline.derivatives(t, n=1), np.linspace(start_width, end_width, count)
         ):
             normal = Vec2(derivative).orthogonal(True)
             curve_trace._append(Vec2(point), normal, width)
         return curve_trace
 
     @classmethod
@@ -460,36 +444,30 @@
             yield from trace.faces()
 
     def faces_wcs(self, ocs: OCS, elevation: float) -> Iterable[Sequence[Vec3]]:
         """Yields all faces as 4-tuples of :class:`~ezdxf.math.Vec3` objects
         in :ref:`WCS`.
         """
         for face in self.faces():
-            yield tuple(
-                ocs.points_to_wcs(Vec3(v.x, v.y, elevation) for v in face)
-            )
+            yield tuple(ocs.points_to_wcs(Vec3(v.x, v.y, elevation) for v in face))
 
     def polygons(self) -> Iterable[Polygon]:
         """Yields for each sub-trace a single polygon as sequence of
         :class:`~ezdxf.math.Vec2` objects in :ref:`OCS`.
         """
         for trace in self._traces:
             yield trace.polygon()
 
-    def polygons_wcs(
-        self, ocs: OCS, elevation: float
-    ) -> Iterable[Sequence[Vec3]]:
+    def polygons_wcs(self, ocs: OCS, elevation: float) -> Iterable[Sequence[Vec3]]:
         """Yields for each sub-trace a single polygon as sequence of
         :class:`~ezdxf.math.Vec3` objects in :ref:`WCS`.
         """
         for trace in self._traces:
             yield tuple(
-                ocs.points_to_wcs(
-                    Vec3(v.x, v.y, elevation) for v in trace.polygon()
-                )
+                ocs.points_to_wcs(Vec3(v.x, v.y, elevation) for v in trace.polygon())
             )
 
     def virtual_entities(
         self, dxftype="TRACE", dxfattribs=None, doc: Optional[Drawing] = None
     ) -> Iterable[Quadrilateral]:
         """Yields faces as SOLID, TRACE or 3DFACE entities with DXF attributes
         given in `dxfattribs`.
@@ -513,26 +491,22 @@
             yield from trace.virtual_entities(dxftype, dxfattribs, doc)
 
     def close(self):
         """Close multi traces by merging first and last trace, if linear traces."""
         traces = self._traces
         if len(traces) < 2:
             return
-        if isinstance(traces[0], LinearTrace) and isinstance(
-            traces[-1], LinearTrace
-        ):
+        if isinstance(traces[0], LinearTrace) and isinstance(traces[-1], LinearTrace):
             first = cast(LinearTrace, traces.pop(0))
             last = cast(LinearTrace, traces[-1])
             for point, start_width, end_width in first:
                 last.add_station(point, start_width, end_width)
 
     @classmethod
-    def from_polyline(
-        cls, polyline: DXFGraphic, segments: int = 64
-    ) -> TraceBuilder:
+    def from_polyline(cls, polyline: DXFGraphic, segments: int = 64) -> TraceBuilder:
         """
         Create a complete trace from a LWPOLYLINE or a 2D POLYLINE entity, the
         trace consist of multiple sub-traces if :term:`bulge` values are
         present. Uses only the :ref:`OCS` coordinates!
 
         Args:
             polyline: :class:`~ezdxf.entities.LWPolyline` or 2D
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py` & `ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,15 @@
 
         def load_block_record(
             block: Block,
             endblk: EndBlk,
             block_entities: list[DXFEntity],
         ) -> BlockRecord:
             try:
-                block_record = cast(
-                    "BlockRecord", block_records.get(block.dxf.name)
-                )
+                block_record = cast("BlockRecord", block_records.get(block.dxf.name))
             # Special case DXF R12 - has no BLOCK_RECORD table
             except DXFTableEntryError:
                 block_record = cast(
                     "BlockRecord",
                     block_records.new(block.dxf.name, dxfattribs={"scale": 0}),
                 )
 
@@ -146,20 +144,19 @@
                 # the block layout, linked entities ares stored in their
                 # parent entity e.g. VERTEX -> POLYLINE:
                 if not linked(entity):
                     yield entity
 
         block_records = self.block_records
         section_head = cast("DXFTagStorage", entities[0])
-        if section_head.dxftype() != "SECTION" or section_head.base_class[
-            1
-        ] != (2, "BLOCKS"):
-            raise DXFStructureError(
-                "Critical structure error in BLOCKS section."
-            )
+        if section_head.dxftype() != "SECTION" or section_head.base_class[1] != (
+            2,
+            "BLOCKS",
+        ):
+            raise DXFStructureError("Critical structure error in BLOCKS section.")
         # Remove SECTION entity
         del entities[0]
         content: list["DXFEntity"] = []
         block: Block = _MISSING_BLOCK_
         for entity in link_entities():
             if isinstance(entity, Block):
                 if block is not _MISSING_BLOCK_:
@@ -218,18 +215,15 @@
         block_layout = BlockLayout(block_record)
         block_record.block_layout = block_layout
         assert self.block_records.has_entry(block_record.dxf.name)
         return block_layout
 
     def __iter__(self) -> Iterator[BlockLayout]:
         """Iterable of all :class:`~ezdxf.layouts.BlockLayout` objects."""
-        return (
-            block_record.block_layout
-            for block_record in self.block_records
-        )
+        return (block_record.block_layout for block_record in self.block_records)
 
     def __contains__(self, name: str) -> bool:
         """Returns ``True`` if :class:`~ezdxf.layouts.BlockLayout` `name`
         exist.
         """
         return self.block_records.has_entry(name)
 
@@ -261,17 +255,15 @@
         `default` if `name` not exist.
         """
         try:
             return self.__getitem__(name)
         except DXFKeyError:
             return default
 
-    def get_block_layout_by_handle(
-        self, block_record_handle: str
-    ) -> BlockLayout:
+    def get_block_layout_by_handle(self, block_record_handle: str) -> BlockLayout:
         """Returns a block layout by block record handle. (internal API)"""
         return self.doc.entitydb[block_record_handle].block_layout  # type: ignore
 
     def new(
         self,
         name: str,
         base_point: UVec = NULLVEC,
@@ -368,17 +360,15 @@
         """
         if safe:
             if is_special_block(name):
                 raise DXFBlockInUseError(
                     f'Special block "{name}" maybe used without explicit INSERT entity.'
                 )
             assert self.doc is not None
-            block_refs = self.doc.query(
-                f"INSERT[name=='{name}']i"
-            )  # ignore case
+            block_refs = self.doc.query(f"INSERT[name=='{name}']i")  # ignore case
             if len(block_refs):
                 raise DXFBlockInUseError(f'Block "{name}" is still in use.')
         self.__delitem__(name)
 
     def delete_all_blocks(self) -> None:
         """Delete all blocks without references except modelspace- or
         paperspace layout blocks, special arrow- and anonymous blocks
@@ -424,15 +414,19 @@
             to delete invalid entities after auditing automatically.
 
         """
         assert self.doc is auditor.doc, "Auditor for different DXF document."
 
         for block_record in self.block_records:
             assert isinstance(block_record, BlockRecord)
-            for entity in block_record.entity_space:
+
+            block_record_handle: str = block_record.dxf.handle
+            unlink_entities: list[DXFEntity] = []
+            es = block_record.entity_space
+            for entity in es:
                 if not is_graphic_entity(entity):
                     auditor.fixed_error(
                         code=AuditError.REMOVED_INVALID_GRAPHIC_ENTITY,
                         message=f"Removed invalid DXF entity {str(entity)} from"
                         f" BLOCK '{block_record.dxf.name}'.",
                     )
                     auditor.trash(entity)
@@ -441,7 +435,27 @@
                     # entity!
                     auditor.fixed_error(
                         code=AuditError.REMOVED_STANDALONE_ATTRIB_ENTITY,
                         message=f"Removed standalone {str(entity)} entity from"
                         f" BLOCK '{block_record.dxf.name}'.",
                     )
                     auditor.trash(entity)
+
+                if not entity.is_alive:
+                    continue
+
+                if entity.dxf.owner != block_record_handle:
+                    auditor.fixed_error(
+                        code=AuditError.REMOVED_ENTITY_WITH_INVALID_OWNER_HANDLE,
+                        message=f"Removed DXF entity {str(entity)} with invalid owner "
+                        f"handle (#{entity.dxf.owner} != #{block_record_handle}) "
+                        f"from BLOCK '{block_record.dxf.name}'.",
+                    )
+                    # do not destroy the entity, it's maybe owned to another block
+                    unlink_entities.append(entity)
+
+            for entity in unlink_entities:
+                if entity.is_alive:
+                    try:
+                        es.remove(entity)
+                    except ValueError:
+                        pass
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/header.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/table.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py` & `ezdxf-1.3.1b0/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,20 +65,20 @@
 
     """
 
     @abc.abstractmethod
     def bbox(self) -> BoundingBox2d: ...
 
     @abc.abstractmethod
-    def is_completley_inside(self, other: BoundingBox2d) -> bool: ...
+    def is_completely_inside(self, other: BoundingBox2d) -> bool: ...
 
     # returning False means: I don't know!
 
     @abc.abstractmethod
-    def is_completley_outside(self, other: BoundingBox2d) -> bool: ...
+    def is_completely_outside(self, other: BoundingBox2d) -> bool: ...
 
     @abc.abstractmethod
     def clip_point(self, point: Vec2) -> Optional[Vec2]: ...
 
     @abc.abstractmethod
     def clip_line(self, start: Vec2, end: Vec2) -> Sequence[tuple[Vec2, Vec2]]: ...
 
@@ -244,48 +244,48 @@
 
     def clip_line(self, start: Vec2, end: Vec2) -> Sequence[tuple[Vec2, Vec2]]:
         return self.clipper.clip_line(start, end)
 
     def clip_polyline(self, points: NumpyPoints2d) -> Sequence[NumpyPoints2d]:
         clipper = self.clipper
         polyline_bbox = BoundingBox2d(points.extents())
-        if self.is_completley_outside(polyline_bbox):
+        if self.is_completely_outside(polyline_bbox):
             return tuple()
-        if self.is_completley_inside(polyline_bbox):
+        if self.is_completely_inside(polyline_bbox):
             return (points,)
         return [
             NumpyPoints2d(part)
             for part in clipper.clip_polyline(points.vertices())
             if len(part) > 0
         ]
 
     def clip_polygon(self, points: NumpyPoints2d) -> Sequence[NumpyPoints2d]:
         clipper = self.clipper
         polygon_bbox = BoundingBox2d(points.extents())
-        if self.is_completley_outside(polygon_bbox):
+        if self.is_completely_outside(polygon_bbox):
             return tuple()
-        if self.is_completley_inside(polygon_bbox):
+        if self.is_completely_inside(polygon_bbox):
             return (points,)
         return [
             NumpyPoints2d(part)
             for part in clipper.clip_polygon(points.vertices())
             if len(part) > 0
         ]
 
     def clip_paths(
         self, paths: Iterable[NumpyPath2d], max_sagitta: float
     ) -> Iterator[NumpyPath2d]:
         clipper = self.clipper
         for path in paths:
             for sub_path in path.sub_paths():
                 path_bbox = BoundingBox2d(sub_path.control_vertices())
-                if self.is_completley_inside(path_bbox):
+                if self.is_completely_inside(path_bbox):
                     yield sub_path
                     continue
-                if self.is_completley_outside(path_bbox):
+                if self.is_completely_outside(path_bbox):
                     continue
                 polyline = Vec2.list(sub_path.flattening(max_sagitta, segments=4))
                 for part in clipper.clip_polyline(polyline):
                     if len(part) > 0:
                         yield NumpyPath2d.from_vertices(part, close=False)
 
     def clip_filled_paths(
@@ -293,18 +293,18 @@
     ) -> Iterator[NumpyPath2d]:
         clipper = self.clipper
         for path in paths:
             for sub_path in path.sub_paths():
                 if len(sub_path) < 2:
                     continue
                 path_bbox = BoundingBox2d(sub_path.control_vertices())
-                if self.is_completley_inside(path_bbox):
+                if self.is_completely_inside(path_bbox):
                     yield sub_path
                     continue
-                if self.is_completley_outside(path_bbox):
+                if self.is_completely_outside(path_bbox):
                     continue
                 for part in clipper.clip_polygon(
                     Vec2.list(sub_path.flattening(max_sagitta, segments=4))
                 ):
                     if len(part) > 0:
                         yield NumpyPath2d.from_vertices(part, close=True)
 
@@ -324,18 +324,18 @@
         if not bbox.has_data:
             raise ValueError("clipping box not detectable")
         size: Vec2 = bbox.size
         self.remove_all = size.x * size.y < 1e-9
 
         super().__init__(bbox, ClippingRect2d(bbox.extmin, bbox.extmax))
 
-    def is_completley_inside(self, other: BoundingBox2d) -> bool:
+    def is_completely_inside(self, other: BoundingBox2d) -> bool:
         return self._bbox.contains(other)
 
-    def is_completley_outside(self, other: BoundingBox2d) -> bool:
+    def is_completely_outside(self, other: BoundingBox2d) -> bool:
         return not self._bbox.has_intersection(other)
 
     def clip_point(self, point: Vec2) -> Optional[Vec2]:
         if self.remove_all:
             return None
         return super().clip_point(point)
 
@@ -377,18 +377,18 @@
 
     def __init__(self, vertices: Iterable[UVec]) -> None:
         from ezdxf.math.clipping import ConvexClippingPolygon2d
 
         polygon = Vec2.list(vertices)
         super().__init__(BoundingBox2d(polygon), ConvexClippingPolygon2d(polygon))
 
-    def is_completley_inside(self, other: BoundingBox2d) -> bool:
+    def is_completely_inside(self, other: BoundingBox2d) -> bool:
         return False  # I don't know!
 
-    def is_completley_outside(self, other: BoundingBox2d) -> bool:
+    def is_completely_outside(self, other: BoundingBox2d) -> bool:
         return not self._bbox.has_intersection(other)
 
 
 class ConcaveClippingPolygon(ClippingPolygon):
     """Represents an arbitrary concave polygon as clipping shape.  Removes the geometry
     outside the clipping polygon.
 
@@ -396,18 +396,18 @@
 
     def __init__(self, vertices: Iterable[UVec]) -> None:
         from ezdxf.math.clipping import ConcaveClippingPolygon2d
 
         polygon = Vec2.list(vertices)
         super().__init__(BoundingBox2d(polygon), ConcaveClippingPolygon2d(polygon))
 
-    def is_completley_inside(self, other: BoundingBox2d) -> bool:
+    def is_completely_inside(self, other: BoundingBox2d) -> bool:
         return False  # I don't know!
 
-    def is_completley_outside(self, other: BoundingBox2d) -> bool:
+    def is_completely_outside(self, other: BoundingBox2d) -> bool:
         return not self._bbox.has_intersection(other)
 
 
 class InvertedClippingPolygon(ClippingPolygon):
     """Represents an arbitrary inverted clipping polygon.  Removes the geometry
     inside the clipping polygon.
 
@@ -415,19 +415,19 @@
 
     def __init__(self, vertices: Iterable[UVec], outer_bounds: BoundingBox2d) -> None:
         from ezdxf.math.clipping import InvertedClippingPolygon2d
 
         polygon = Vec2.list(vertices)
         super().__init__(outer_bounds, InvertedClippingPolygon2d(polygon, outer_bounds))
 
-    def is_completley_inside(self, other: BoundingBox2d) -> bool:
+    def is_completely_inside(self, other: BoundingBox2d) -> bool:
         # returning False means: I don't know!
         return False  # not easy to detect
 
-    def is_completley_outside(self, other: BoundingBox2d) -> bool:
+    def is_completely_outside(self, other: BoundingBox2d) -> bool:
         return not self._bbox.has_intersection(other)
 
 
 def find_best_clipping_shape(polygon: Iterable[UVec]) -> ClippingShape:
     """Returns the best clipping shape for the given clipping polygon.
 
     The function analyses the given polygon (rectangular, convex or concave polygon, ...)
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/test.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/text.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py` & `ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.0rc0
+Version: 1.3.1b0
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,22 +101,26 @@
 src/ezdxf/colors.py
 src/ezdxf/commands.py
 src/ezdxf/comments.py
 src/ezdxf/disassemble.py
 src/ezdxf/document.py
 src/ezdxf/dwginfo.py
 src/ezdxf/dynblkhelper.py
+src/ezdxf/edgeminer.py
+src/ezdxf/edgesmith.py
 src/ezdxf/entitydb.py
 src/ezdxf/enums.py
 src/ezdxf/explode.py
 src/ezdxf/eztypes.py
 src/ezdxf/filemanagement.py
 src/ezdxf/gfxattribs.py
 src/ezdxf/graphicsfactory.py
 src/ezdxf/groupby.py
+src/ezdxf/messenger.py
+src/ezdxf/msgtypes.py
 src/ezdxf/npshapes.py
 src/ezdxf/protocols.py
 src/ezdxf/proxygraphic.py
 src/ezdxf/py.typed
 src/ezdxf/query.py
 src/ezdxf/queryparser.py
 src/ezdxf/r12strict.py
@@ -151,22 +155,24 @@
 src/ezdxf/acc/matrix44.pyx
 src/ezdxf/acc/np_support.pyx
 src/ezdxf/acc/vector.pxd
 src/ezdxf/acc/vector.pyx
 src/ezdxf/acis/__init__.py
 src/ezdxf/acis/abstract.py
 src/ezdxf/acis/api.py
+src/ezdxf/acis/cache.py
 src/ezdxf/acis/const.py
 src/ezdxf/acis/dbg.py
 src/ezdxf/acis/dxf.py
 src/ezdxf/acis/entities.py
 src/ezdxf/acis/hdr.py
 src/ezdxf/acis/mesh.py
 src/ezdxf/acis/sab.py
 src/ezdxf/acis/sat.py
+src/ezdxf/acis/type_hints.py
 src/ezdxf/addons/__init__.py
 src/ezdxf/addons/acadctb.py
 src/ezdxf/addons/binpacking.py
 src/ezdxf/addons/dimlines.py
 src/ezdxf/addons/dxf2code.py
 src/ezdxf/addons/genetic_algorithm.py
 src/ezdxf/addons/geo.py
@@ -694,14 +700,17 @@
 tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 tests/test_05_tools/test_539_npshapes.py
 tests/test_05_tools/test_540_lff_parser.py
 tests/test_05_tools/test_541_clipping_portal.py
 tests/test_05_tools/test_542_itertools.py
 tests/test_05_tools/test_543_select.py
 tests/test_05_tools/test_544_revcloud.py
+tests/test_05_tools/test_545_acis_cache.py
+tests/test_05_tools/test_546_edgeminer.py
+tests/test_05_tools/test_547_edgesmith.py
 tests/test_06_math/conftest.py
 tests/test_06_math/test_600_base.py
 tests/test_06_math/test_601_bulge.py
 tests/test_06_math/test_602_vec3.py
 tests/test_06_math/test_603_vec2.py
 tests/test_06_math/test_604_banded_matrix.py
 tests/test_06_math/test_604_linalg.py
@@ -808,13 +817,14 @@
 tests/test_08_addons/test_827_geojson_backend.py
 tests/test_09_cython_acceleration/test_901_acc_vec2.py
 tests/test_09_cython_acceleration/test_902_acc_vec3.py
 tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 tests/test_09_cython_acceleration/test_906_acc_bspline.py
+tests/test_10_issues/test_issue_1078_bbox_calculation.py
 tests/test_10_issues/test_issue_414_bbox_calculation.py
 tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 tests/test_10_issues/test_issue_574_flattening_error.py
 tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
 tests/test_10_issues/test_issue_749_text_layout.py
 tests/test_10_issues/test_issue_873_circle_inverted_normal.py
```

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py` & `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py` & `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2015-2019, Manfred Moitzi
+# Copyright (c) 2015-2024, Manfred Moitzi
 # License: MIT License
 import pytest
 import ezdxf
 
 
 @pytest.fixture(scope="module")
 def groups():
@@ -60,15 +60,45 @@
     # or in a block
     msp = dwg.modelspace()
     with group.edit_data() as e:  # e is a standard Python list of DXF entities
         line = msp.add_line((0, 0), (3, 0))
         e.append(line)
         e.append(msp.add_circle((0, 0), radius=2))
 
-    assert 2 == len(group)
+    assert len(group) == 2
     assert line in group
 
-    ungrouped_line = msp.add_line((0, 1), (3, 1))
-    assert ungrouped_line not in group
+    group_handle = group.dxf.handle
+    for entity in group:
+        assert (
+            group_handle in entity.reactors
+        ), "expected group handle as reactor in entity"
 
     group.clear()
-    assert 0 == len(group)
+    assert len(group) == 0
+    assert (
+        group_handle not in line.reactors
+    ), "group handle has to be removed from reactors"
+
+
+def test_extend_group():
+    dwg = ezdxf.new("R2000")
+    group = dwg.groups.new()
+    group_handle = group.dxf.handle
+    # the group itself is not an entity space, DXF entities has to be placed in model space, paper space
+    # or in a block
+    msp = dwg.modelspace()
+    line = msp.add_line((0, 0), (3, 0))
+    group.set_data([line])
+    assert len(group) == 1
+
+    line2 = msp.add_line((0, 0), (3, 0))
+    group.extend([line2])
+    assert len(group) == 2
+    assert group_handle in line2.reactors, "expected group handle as reactor in entity"
+
+    group.extend([line])
+    assert len(group) == 2, "cannot add same entity a second time"
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232d_acis_copy.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232e_acis_transform.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files 21% similar despite different names*

```diff
@@ -177,9 +177,45 @@
     paths.edge_to_polyline_paths(distance=0.1)
     path = paths[0]
     assert path.type == BoundaryPathType.POLYLINE
     assert path.has_bulge() is False
     assert len(path.vertices) == 5
 
 
+class TestValidatingBoundaryPaths:
+    def test_spline_edge_has_valid_knot_count(self):
+        paths = BoundaryPaths()
+        edge_path = paths.add_edge_path()
+        spline = edge_path.add_spline(
+            control_points=[(0, 0), (1, 1), (2, 0), (3, 1)],
+            knot_values=[1, 2, 3, 4, 5, 6, 7, 8],
+        )
+        assert spline.is_valid() is True, "expected degree + count + 1 values"
+
+        spline.knot_values = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+        assert spline.is_valid() is False, "too many knot value"
+        spline.knot_values = [0, 0, 0, 0]
+        assert spline.is_valid() is False, "too few knot value"
+        
+        assert paths.is_valid() is False, "invalid state should be propagated"
+
+    def test_spline_edge_has_enough_control_points(self):
+        paths = BoundaryPaths()
+        edge_path = paths.add_edge_path()
+        spline = edge_path.add_spline(
+            control_points=[(0, 0), (1, 1), (2, 0)],
+            knot_values=[1, 2, 3, 4, 5, 6, 7],  # correct degree + count + 1!
+        )
+        assert spline.is_valid() is False, "too few control points"
+
+    def test_spline_edge_has_enough_fir_points(self):
+        paths = BoundaryPaths()
+        edge_path = paths.add_edge_path()
+        spline = edge_path.add_spline(
+            fit_points=[(0, 0), (1, 1), (2, 0)],
+        )
+        assert spline.is_valid() is True, "expected 2 or more points"
+        spline.fit_points = [(0, 0)]
+        assert spline.is_valid() is False, "too few fit points"
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,16 @@
     msp = doc.modelspace()
     block = doc.blocks.new("Block6")
     point1 = block.add_point((0, 0))  # invalid BLOCK entity
     point2 = msp.add_point((0, 0))  # valid model space entity ...
     point2.destroy()  # ... but destroyed
     layer = doc.layers.get("0")  # invalid table entry
 
-    group.extend([point1, point2, layer])
+    # hack, hack, hack - but since 2024-05-23 group.extend() validates the input data!
+    group._data.extend([point1, point2, layer])
     auditor = Auditor(doc)
     group.audit(auditor)
     assert len(group) == 0
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,7 +223,28 @@
     line = msp.add_line((0, 0), (1, 0))
     # transparency value requires 0x02000000 bit set
     line.dxf.unprotected_set("transparency", 0x10000000)
     auditor = Auditor(doc)
     line.audit(auditor)
     assert line.dxf.hasattr("transparency") is False
     assert len(auditor.fixes) == 1
+
+
+def test_fix_entities_with_invalid_owner_handle():
+    doc = ezdxf.new()
+    msp = doc.modelspace()
+    line = msp.add_line((0, 0), (1, 0))
+
+    block = doc.blocks.new("TEST")
+    block.add_entity(line)
+
+    result = doc.audit()
+    fix = result.fixes[0]
+    assert fix.code == AuditError.REMOVED_ENTITY_WITH_INVALID_OWNER_HANDLE
+
+    assert len(block) == 1
+    assert len(msp) == 0
+    assert line.dxf.owner == block.dxf.handle
+
+
+if __name__ == '__main__':
+    pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py` & `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py` & `ezdxf-1.3.1b0/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  Copyright (c) 2022, Manfred Moitzi
 #  License: MIT License
 from typing import cast
 import pytest
 import math
-from ezdxf.acis.api import mesh_from_body, load, body_from_mesh
+from ezdxf.acis.api import mesh_from_body, load, body_from_mesh, vertices_from_body
 from ezdxf.acis.mesh import PolyhedronFaceBuilder
 from ezdxf.acis import entities, dbg
 from ezdxf.render import forms
 from ezdxf.math import BoundingBox, Vec3
 
 
 class TestPrismToMesh:
@@ -43,18 +43,15 @@
         assert len(builder.acis_faces()) == 6
 
     def test_each_face_gets_it_own_plane(self, builder):
         """Each face has to have its own flat surface plane."""
         planes = {id(face.surface) for face in builder.acis_faces()}
         assert len(planes) == 6
         assert (
-            all(
-                face.surface.type == "plane-surface"
-                for face in builder.acis_faces()
-            )
+            all(face.surface.type == "plane-surface" for face in builder.acis_faces())
             is True
         )
 
     def test_each_face_has_a_single_loop(self, builder):
         """The PolyhedronFaceBuilder supports only a single loop for each face,
         so divided faces or holes in faces are not supported.
         """
@@ -206,9 +203,20 @@
 
     sponge = MengerSponge().mesh()
     body = body_from_mesh(sponge)
     debugger = dbg.AcisDebugger(body)
     assert debugger.is_manifold() is True
 
 
+def test_vertices_from_body():
+    cube = forms.cube()
+    body = body_from_mesh(cube)
+    vertices = vertices_from_body(body)
+    extents = BoundingBox(vertices)
+
+    assert extents.extmin.isclose((-0.5, -0.5, -0.5))
+    assert extents.extmax.isclose((0.5, 0.5, 0.5))
+    assert len(vertices) == 6 * 4 * 2  # 6 faces x 4 edges x 2 vertices
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py` & `ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/conftest.py` & `ezdxf-1.3.1b0/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py` & `ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (c) 2019 Manfred Moitzi
 # License: MIT License
+import pytest
 import ezdxf
 from ezdxf.addons.dxf2code import (
     entities_to_code,
     table_entries_to_code,
     block_to_code,
 )
 from ezdxf.addons.dxf2code import (
     _fmt_mapping,
     _fmt_list,
     _fmt_api_call,
     _fmt_dxf_tags,
 )
 
+import ezdxf.entities
 from ezdxf.lldxf.types import dxftag
 from ezdxf.lldxf.tags import Tags  # required by exec() or eval()
 from ezdxf.entities.ltype import LinetypePattern  # required by exec() or eval()
 from ezdxf.math import Vec3
 
 doc = ezdxf.new("R2010")
 msp = doc.modelspace()
@@ -446,7 +448,26 @@
     block = testdoc.blocks.new("TestBlock", dxfattribs={"description": "test"})
     block.add_line((1, 1), (2, 2))
     code = block_to_code(block, drawing="doc")
     exec(str(code), globals())
     new_block = doc.blocks.get("TestBlock")
     assert new_block.block.dxf.description == block.block.dxf.description
     assert new_block[0].dxftype() == block[0].dxftype()
+
+
+def test_hatch_to_code():
+    from ezdxf.entities import Hatch
+
+    hatch = Hatch()
+    hatch.set_pattern_fill(name="ANGLE")
+    hatch.paths.add_polyline_path(
+        [(0, 0), (100, 0), (100, 100), (0, 100)], is_closed=True
+    )
+
+    new_hatch = translate_to_code_and_execute(hatch)
+    assert isinstance(new_hatch, Hatch)
+    assert new_hatch.has_pattern_fill
+    assert len(new_hatch.pattern.lines) == len(hatch.pattern.lines)
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Created: 24.03.2010
-# Copyright (c) 2010-2019, Manfred Moitzi
+# Copyright (c) 2010-2024, Manfred Moitzi
 # License: MIT License
 import pytest
 
 import os
 import math
 from ezdxf.addons.acadctb import *
 
@@ -146,17 +145,15 @@
     def test_set_table_lineweight(self, styles):
         styles.set_table_lineweight(7, 1.70)
         assert math.isclose(styles.get_table_lineweight(7), 1.70, abs_tol=1e-6)
 
     def test_set_table_lineweight_index_error(self, styles):
         index_out_of_range = len(styles.lineweights) + 7
         index = styles.set_table_lineweight(index_out_of_range, 7.77)
-        assert math.isclose(
-            styles.get_table_lineweight(index), 7.77, abs_tol=1e-6
-        )
+        assert math.isclose(styles.get_table_lineweight(index), 7.77, abs_tol=1e-6)
 
     def test_write_header(self):
         expected = (
             'description="\n'
             "aci_table_available=TRUE\n"
             "scale_factor=1.0\n"
             "apply_factor=FALSE\n"
@@ -168,17 +165,15 @@
         result = fp.getvalue()
         fp.close()
         assert result == expected
 
     def test_write_aci_table(self):
         expected = (
             "aci_table{\n"
-            + "\n".join(
-                (' %s="Color_%d' % (index, index + 1) for index in range(255))
-            )
+            + "\n".join((' %s="Color_%d' % (index, index + 1) for index in range(255)))
             + "\n}\n"
         )
         styles = ColorDependentPlotStyles()
         fp = StringIO()
         styles._write_aci_table(fp)
         result = fp.getvalue()
         fp.close()
@@ -432,7 +427,32 @@
 
     def test_get_bool(self):
         assert get_bool(True)
         assert get_bool("true")
         assert get_bool(False) is False
         assert get_bool("false") is False
         pytest.raises(ValueError, get_bool, "falsch")
+
+
+def test_parser_ignores_unknown_appendix():
+    parser = PlotStyleFileParser(
+        r"""custom_lineweight_table{
+ 0=0.0076200000000 (+7.Z+"8V?S_LC )
+ 1=0.0254
+ 6=0.17780000000   (  44F=@";"QC\\SM0)
+ 7=0.2
+ 10=0.35560000000 (44F=@";"UC_SN )
+ 11=0.4
+}
+"""
+    )
+    table = parser.get("custom_lineweight_table", {})
+    assert table["0"] == "0.0076200000000"
+    assert table["1"] == "0.0254"
+    assert table["6"] == "0.17780000000"
+    assert table["7"] == "0.2"
+    assert table["10"] == "0.35560000000"
+    assert table["11"] == "0.4"
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py` & `ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*


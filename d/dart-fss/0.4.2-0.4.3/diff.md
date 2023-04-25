# Comparing `tmp/dart-fss-0.4.2.tar.gz` & `tmp/dart-fss-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-fss-0.4.2.tar", last modified: Tue Mar  7 10:58:04 2023, max compression
+gzip compressed data, was "dart-fss-0.4.3.tar", last modified: Tue Apr 25 00:35:23 2023, max compression
```

## Comparing `dart-fss-0.4.2.tar` & `dart-fss-0.4.3.tar`

### file list

```diff
@@ -1,157 +1,180 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:04.116412 dart-fss-0.4.2/
--rw-rw-rw-   0        0        0     1093 2023-03-07 10:57:31.000000 dart-fss-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       77 2023-03-07 10:57:31.000000 dart-fss-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3058 2023-03-07 10:58:04.116412 dart-fss-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2401 2023-03-07 10:57:31.000000 dart-fss-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:04.116412 dart-fss-0.4.2/dart_fss/
--rw-rw-rw-   0        0        0      619 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/__init__.py
--rw-rw-rw-   0        0        0      518 2023-03-07 10:58:04.116412 dart-fss-0.4.2/dart_fss/_version.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.330693 dart-fss-0.4.2/dart_fss/api/
--rw-rw-rw-   0        0        0      224 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.361959 dart-fss-0.4.2/dart_fss/api/filings/
--rw-rw-rw-   0        0        0      260 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/filings/__init__.py
--rw-rw-rw-   0        0        0      396 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/filings/company.py
--rw-rw-rw-   0        0        0     1320 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/filings/corp_code.py
--rw-rw-rw-   0        0        0      686 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/filings/document.py
--rw-rw-rw-   0        0        0     2680 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/filings/search_filings.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.393209 dart-fss-0.4.2/dart_fss/api/finance/
--rw-rw-rw-   0        0        0      394 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/fnltt_multi_acnt.py
--rw-rw-rw-   0        0        0     1183 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/fnltt_singl_acnt.py
--rw-rw-rw-   0        0        0     1272 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/fnltt_singl_acnt_all.py
--rw-rw-rw-   0        0        0     1349 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/xbrl.py
--rw-rw-rw-   0        0        0      774 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/finance/xbrl_taxonomy.py
--rw-rw-rw-   0        0        0     3692 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/helper.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.549456 dart-fss-0.4.2/dart_fss/api/info/
--rw-rw-rw-   0        0        0     2590 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/__init__.py
--rw-rw-rw-   0        0        0     1184 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py
--rw-rw-rw-   0        0        0     1229 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py
--rw-rw-rw-   0        0        0     1132 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/adt_servc_cncls_sttus.py
--rw-rw-rw-   0        0        0     1112 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/alot_matter.py
--rw-rw-rw-   0        0        0     1173 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1127 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/cprnd_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1134 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/det_scrits_isu_acmslt.py
--rw-rw-rw-   0        0        0     1258 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py
--rw-rw-rw-   0        0        0     1271 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py
--rw-rw-rw-   0        0        0     1088 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/emp_sttus.py
--rw-rw-rw-   0        0        0     1169 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1092 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/exctv_sttus.py
--rw-rw-rw-   0        0        0     1154 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/hmv_audit_all_sttus.py
--rw-rw-rw-   0        0        0     1173 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py
--rw-rw-rw-   0        0        0     1123 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/hyslr_chg_sttus.py
--rw-rw-rw-   0        0        0     1104 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/hyslr_sttus.py
--rw-rw-rw-   0        0        0     1174 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/indvdl_by_pay.py
--rw-rw-rw-   0        0        0     1106 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/irds_sttus.py
--rw-rw-rw-   0        0        0     1102 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/mrhl_sttus.py
--rw-rw-rw-   0        0        0     1163 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1130 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/otr_cpr_invstmnt_sttus.py
--rw-rw-rw-   0        0        0     1167 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py
--rw-rw-rw-   0        0        0     1140 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/prvsrp_cptal_use_dtls.py
--rw-rw-rw-   0        0        0     1138 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/pssrp_cptal_use_dtls.py
--rw-rw-rw-   0        0        0     1146 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py
--rw-rw-rw-   0        0        0     1121 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/stock_totqy_sttus.py
--rw-rw-rw-   0        0        0     1160 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/tesstk_acqs_dsps_sttus.py
--rw-rw-rw-   0        0        0     1146 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/info/unrst_exctv_mendng_sttus.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.752753 dart-fss-0.4.2/dart_fss/api/issue/
--rw-rw-rw-   0        0        0     2421 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/__init__.py
--rw-rw-rw-   0        0        0     1115 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py
--rw-rw-rw-   0        0        0     1103 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bdwt_is_decsn.py
--rw-rw-rw-   0        0        0     1101 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bnk_mngt_pcbg.py
--rw-rw-rw-   0        0        0     1101 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bnk_mngt_pcsp.py
--rw-rw-rw-   0        0        0     1061 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bsn_inh_decsn.py
--rw-rw-rw-   0        0        0     1034 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bsn_sp.py
--rw-rw-rw-   0        0        0     1061 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/bsn_trf_decsn.py
--rw-rw-rw-   0        0        0     1059 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/cmp_dv_decsn.py
--rw-rw-rw-   0        0        0     1075 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/cmp_dvmg_decsn.py
--rw-rw-rw-   0        0        0     1059 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/cmp_mg_decsn.py
--rw-rw-rw-   0        0        0     1040 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/cr_decsn.py
--rw-rw-rw-   0        0        0     1070 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ctrcvs_bgrq.py
--rw-rw-rw-   0        0        0     1079 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/cvbd_is_decsn.py
--rw-rw-rw-   0        0        0     1034 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/df_ocr.py
--rw-rw-rw-   0        0        0     1053 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ds_rs_ocr.py
--rw-rw-rw-   0        0        0     1079 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/exbd_is_decsn.py
--rw-rw-rw-   0        0        0     1056 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/fric_decsn.py
--rw-rw-rw-   0        0        0     1052 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/lwst_lg.py
--rw-rw-rw-   0        0        0     1139 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py
--rw-rw-rw-   0        0        0     1139 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py
--rw-rw-rw-   0        0        0     1096 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ov_dlst.py
--rw-rw-rw-   0        0        0     1121 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ov_dlst_decsn.py
--rw-rw-rw-   0        0        0     1082 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ov_lst.py
--rw-rw-rw-   0        0        0     1107 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/ov_lst_decsn.py
--rw-rw-rw-   0        0        0     1066 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/pifric_decsn.py
--rw-rw-rw-   0        0        0     1056 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/piic_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/stk_extr_decsn.py
--rw-rw-rw-   0        0        0     1105 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/stkrtbd_inh_decsn.py
--rw-rw-rw-   0        0        0     1105 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/stkrtbd_trf_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tgast_inh_decsn.py
--rw-rw-rw-   0        0        0     1079 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tgast_trf_decsn.py
--rw-rw-rw-   0        0        0     1077 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_decsn.py
--rw-rw-rw-   0        0        0     1131 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py
--rw-rw-rw-   0        0        0     1133 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py
--rw-rw-rw-   0        0        0     1077 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/tsstk_dp_decsn.py
--rw-rw-rw-   0        0        0     1120 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/issue/wd_cocobd_is_decsn.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.768379 dart-fss-0.4.2/dart_fss/api/market/
--rw-rw-rw-   0        0        0      187 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/market/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/market/stock_market.py
--rw-rw-rw-   0        0        0     2009 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/market/trading_halt.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.799626 dart-fss-0.4.2/dart_fss/api/registration/
--rw-rw-rw-   0        0        0      306 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/bd_rs.py
--rw-rw-rw-   0        0        0     1014 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/dv_rs.py
--rw-rw-rw-   0        0        0     1030 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/estk_rs.py
--rw-rw-rw-   0        0        0     1070 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/extr_rs.py
--rw-rw-rw-   0        0        0     1014 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/mg_rs.py
--rw-rw-rw-   0        0        0     1044 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/registration/stkdp_rs.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.815247 dart-fss-0.4.2/dart_fss/api/shareholder/
--rw-rw-rw-   0        0        0      149 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/shareholder/__init__.py
--rw-rw-rw-   0        0        0      830 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/shareholder/elestock.py
--rw-rw-rw-   0        0        0      794 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/api/shareholder/majorstock.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.839876 dart-fss-0.4.2/dart_fss/auth/
--rw-rw-rw-   0        0        0      124 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/auth/__init__.py
--rw-rw-rw-   0        0        0     2567 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/auth/auth.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.846550 dart-fss-0.4.2/dart_fss/corp/
--rw-rw-rw-   0        0        0      172 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/corp/__init__.py
--rw-rw-rw-   0        0        0     8929 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/corp/corp.py
--rw-rw-rw-   0        0        0     9456 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/corp/corp_list.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.877812 dart-fss-0.4.2/dart_fss/errors/
--rw-rw-rw-   0        0        0      459 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/errors/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/errors/checker.py
--rw-rw-rw-   0        0        0     1744 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.893440 dart-fss-0.4.2/dart_fss/filings/
--rw-rw-rw-   0        0        0       91 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/filings/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/filings/pages.py
--rw-rw-rw-   0        0        0    20300 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/filings/reports.py
--rw-rw-rw-   0        0        0     2513 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/filings/search.py
--rw-rw-rw-   0        0        0     2124 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/filings/search_result.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:04.022669 dart-fss-0.4.2/dart_fss/fs/
--rw-rw-rw-   0        0        0      158 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/fs/__init__.py
--rw-rw-rw-   0        0        0    54845 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/fs/extract.py
--rw-rw-rw-   0        0        0     7924 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/fs/fs.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:04.085164 dart-fss-0.4.2/dart_fss/utils/
--rw-rw-rw-   0        0        0     1277 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/__init__.py
--rw-rw-rw-   0        0        0      842 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/cache.py
--rw-rw-rw-   0        0        0      704 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/dataframe.py
--rw-rw-rw-   0        0        0     1434 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/datetime.py
--rw-rw-rw-   0        0        0     2666 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/file.py
--rw-rw-rw-   0        0        0     2733 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/notebook.py
--rw-rw-rw-   0        0        0     3077 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/regex.py
--rw-rw-rw-   0        0        0     7602 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/request.py
--rw-rw-rw-   0        0        0      304 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/singleton.py
--rw-rw-rw-   0        0        0     1019 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/spinner.py
--rw-rw-rw-   0        0        0     2134 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/utils/string.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:04.100795 dart-fss-0.4.2/dart_fss/xbrl/
--rw-rw-rw-   0        0        0       97 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/xbrl/__init__.py
--rw-rw-rw-   0        0        0    10993 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/xbrl/dart_xbrl.py
--rw-rw-rw-   0        0        0    12749 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/xbrl/helper.py
--rw-rw-rw-   0        0        0     9069 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/xbrl/table.py
--rw-rw-rw-   0        0        0     1441 2023-03-07 10:57:31.000000 dart-fss-0.4.2/dart_fss/xbrl/xbrl.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:58:03.327178 dart-fss-0.4.2/dart_fss.egg-info/
--rw-rw-rw-   0        0        0     3058 2023-03-07 10:58:03.000000 dart-fss-0.4.2/dart_fss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-03-07 10:58:03.000000 dart-fss-0.4.2/dart_fss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 10:58:03.000000 dart-fss-0.4.2/dart_fss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      290 2023-03-07 10:58:03.000000 dart-fss-0.4.2/dart_fss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-07 10:58:03.000000 dart-fss-0.4.2/dart_fss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      320 2023-03-07 10:57:31.000000 dart-fss-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0      186 2023-03-07 10:58:04.116412 dart-fss-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-03-07 10:57:31.000000 dart-fss-0.4.2/setup.py
--rw-rw-rw-   0        0        0    80318 2023-03-07 10:57:31.000000 dart-fss-0.4.2/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.374908 dart-fss-0.4.3/
+-rw-rw-rw-   0        0        0     1093 2023-03-06 00:18:03.000000 dart-fss-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0       77 2023-03-06 00:18:03.000000 dart-fss-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3289 2023-04-25 00:35:23.374908 dart-fss-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2401 2023-04-25 00:23:22.000000 dart-fss-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.377140 dart-fss-0.4.3/dart_fss/
+-rw-rw-rw-   0        0        0      619 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-25 00:35:23.377140 dart-fss-0.4.3/dart_fss/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.893946 dart-fss-0.4.3/dart_fss/api/
+-rw-rw-rw-   0        0        0      224 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.911651 dart-fss-0.4.3/dart_fss/api/filings/
+-rw-rw-rw-   0        0        0      260 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/__init__.py
+-rw-rw-rw-   0        0        0      396 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/company.py
+-rw-rw-rw-   0        0        0     1320 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/corp_code.py
+-rw-rw-rw-   0        0        0      686 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/document.py
+-rw-rw-rw-   0        0        0     2680 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/filings/search_filings.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.932141 dart-fss-0.4.3/dart_fss/api/finance/
+-rw-rw-rw-   0        0        0      394 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_multi_acnt.py
+-rw-rw-rw-   0        0        0     1183 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt.py
+-rw-rw-rw-   0        0        0     1272 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt_all.py
+-rw-rw-rw-   0        0        0     1349 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/xbrl.py
+-rw-rw-rw-   0        0        0      774 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/finance/xbrl_taxonomy.py
+-rw-rw-rw-   0        0        0     3692 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/helper.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.011132 dart-fss-0.4.3/dart_fss/api/info/
+-rw-rw-rw-   0        0        0     2590 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/__init__.py
+-rw-rw-rw-   0        0        0     1184 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py
+-rw-rw-rw-   0        0        0     1229 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py
+-rw-rw-rw-   0        0        0     1132 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/adt_servc_cncls_sttus.py
+-rw-rw-rw-   0        0        0     1112 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/alot_matter.py
+-rw-rw-rw-   0        0        0     1173 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1127 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/cprnd_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1134 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/det_scrits_isu_acmslt.py
+-rw-rw-rw-   0        0        0     1258 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py
+-rw-rw-rw-   0        0        0     1271 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py
+-rw-rw-rw-   0        0        0     1088 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/emp_sttus.py
+-rw-rw-rw-   0        0        0     1169 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1092 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/exctv_sttus.py
+-rw-rw-rw-   0        0        0     1154 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hmv_audit_all_sttus.py
+-rw-rw-rw-   0        0        0     1173 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py
+-rw-rw-rw-   0        0        0     1123 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hyslr_chg_sttus.py
+-rw-rw-rw-   0        0        0     1104 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/hyslr_sttus.py
+-rw-rw-rw-   0        0        0     1174 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/indvdl_by_pay.py
+-rw-rw-rw-   0        0        0     1106 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/irds_sttus.py
+-rw-rw-rw-   0        0        0     1102 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/mrhl_sttus.py
+-rw-rw-rw-   0        0        0     1163 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1130 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/otr_cpr_invstmnt_sttus.py
+-rw-rw-rw-   0        0        0     1167 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py
+-rw-rw-rw-   0        0        0     1140 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/prvsrp_cptal_use_dtls.py
+-rw-rw-rw-   0        0        0     1138 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/pssrp_cptal_use_dtls.py
+-rw-rw-rw-   0        0        0     1146 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py
+-rw-rw-rw-   0        0        0     1121 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/stock_totqy_sttus.py
+-rw-rw-rw-   0        0        0     1160 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/tesstk_acqs_dsps_sttus.py
+-rw-rw-rw-   0        0        0     1146 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/info/unrst_exctv_mendng_sttus.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.113728 dart-fss-0.4.3/dart_fss/api/issue/
+-rw-rw-rw-   0        0        0     2421 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py
+-rw-rw-rw-   0        0        0     1103 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bdwt_is_decsn.py
+-rw-rw-rw-   0        0        0     1101 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcbg.py
+-rw-rw-rw-   0        0        0     1101 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcsp.py
+-rw-rw-rw-   0        0        0     1061 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_inh_decsn.py
+-rw-rw-rw-   0        0        0     1034 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_sp.py
+-rw-rw-rw-   0        0        0     1061 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/bsn_trf_decsn.py
+-rw-rw-rw-   0        0        0     1059 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_dv_decsn.py
+-rw-rw-rw-   0        0        0     1075 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_dvmg_decsn.py
+-rw-rw-rw-   0        0        0     1059 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cmp_mg_decsn.py
+-rw-rw-rw-   0        0        0     1040 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cr_decsn.py
+-rw-rw-rw-   0        0        0     1070 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ctrcvs_bgrq.py
+-rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/cvbd_is_decsn.py
+-rw-rw-rw-   0        0        0     1034 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/df_ocr.py
+-rw-rw-rw-   0        0        0     1053 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ds_rs_ocr.py
+-rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/exbd_is_decsn.py
+-rw-rw-rw-   0        0        0     1056 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/fric_decsn.py
+-rw-rw-rw-   0        0        0     1052 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/lwst_lg.py
+-rw-rw-rw-   0        0        0     1139 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py
+-rw-rw-rw-   0        0        0     1139 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py
+-rw-rw-rw-   0        0        0     1096 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_dlst.py
+-rw-rw-rw-   0        0        0     1121 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_dlst_decsn.py
+-rw-rw-rw-   0        0        0     1082 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_lst.py
+-rw-rw-rw-   0        0        0     1107 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/ov_lst_decsn.py
+-rw-rw-rw-   0        0        0     1066 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/pifric_decsn.py
+-rw-rw-rw-   0        0        0     1056 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/piic_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stk_extr_decsn.py
+-rw-rw-rw-   0        0        0     1105 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_inh_decsn.py
+-rw-rw-rw-   0        0        0     1105 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_trf_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tgast_inh_decsn.py
+-rw-rw-rw-   0        0        0     1079 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tgast_trf_decsn.py
+-rw-rw-rw-   0        0        0     1077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_decsn.py
+-rw-rw-rw-   0        0        0     1131 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py
+-rw-rw-rw-   0        0        0     1133 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py
+-rw-rw-rw-   0        0        0     1077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/tsstk_dp_decsn.py
+-rw-rw-rw-   0        0        0     1120 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/issue/wd_cocobd_is_decsn.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.122301 dart-fss-0.4.3/dart_fss/api/market/
+-rw-rw-rw-   0        0        0      187 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/stock_market.py
+-rw-rw-rw-   0        0        0     2009 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/market/trading_halt.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.145189 dart-fss-0.4.3/dart_fss/api/registration/
+-rw-rw-rw-   0        0        0      306 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/bd_rs.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/dv_rs.py
+-rw-rw-rw-   0        0        0     1030 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/estk_rs.py
+-rw-rw-rw-   0        0        0     1070 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/extr_rs.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/mg_rs.py
+-rw-rw-rw-   0        0        0     1044 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/registration/stkdp_rs.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.155533 dart-fss-0.4.3/dart_fss/api/shareholder/
+-rw-rw-rw-   0        0        0      149 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/elestock.py
+-rw-rw-rw-   0        0        0      794 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/api/shareholder/majorstock.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.156533 dart-fss-0.4.3/dart_fss/auth/
+-rw-rw-rw-   0        0        0      124 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/auth/__init__.py
+-rw-rw-rw-   0        0        0     2567 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/auth/auth.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.163032 dart-fss-0.4.3/dart_fss/corp/
+-rw-rw-rw-   0        0        0      172 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/__init__.py
+-rw-rw-rw-   0        0        0     8929 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/corp.py
+-rw-rw-rw-   0        0        0     9456 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/corp/corp_list.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.176629 dart-fss-0.4.3/dart_fss/errors/
+-rw-rw-rw-   0        0        0      459 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/checker.py
+-rw-rw-rw-   0        0        0     1744 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.192675 dart-fss-0.4.3/dart_fss/filings/
+-rw-rw-rw-   0        0        0       91 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/pages.py
+-rw-rw-rw-   0        0        0    20300 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/reports.py
+-rw-rw-rw-   0        0        0     2513 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/search.py
+-rw-rw-rw-   0        0        0     2124 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/filings/search_result.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.257027 dart-fss-0.4.3/dart_fss/fs/
+-rw-rw-rw-   0        0        0      158 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/fs/__init__.py
+-rw-rw-rw-   0        0        0    54845 2023-03-06 00:19:24.000000 dart-fss-0.4.3/dart_fss/fs/extract.py
+-rw-rw-rw-   0        0        0     7924 2023-04-24 06:22:06.000000 dart-fss-0.4.3/dart_fss/fs/fs.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.313837 dart-fss-0.4.3/dart_fss/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_filings.py
+-rw-rw-rw-   0        0        0     1721 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_finance.py
+-rw-rw-rw-   0        0        0    10350 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_info.py
+-rw-rw-rw-   0        0        0    12724 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_issue.py
+-rw-rw-rw-   0        0        0      182 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_market.py
+-rw-rw-rw-   0        0        0     2136 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_registration.py
+-rw-rw-rw-   0        0        0      644 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_api_shareholder.py
+-rw-rw-rw-   0        0        0       88 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.321005 dart-fss-0.4.3/dart_fss/tests/test_case/
+-rw-rw-rw-   0        0        0     5306 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_case/crp_case.py
+-rw-rw-rw-   0        0        0     2998 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_case/testcrp.py
+-rw-rw-rw-   0        0        0     2637 2023-03-07 00:59:43.000000 dart-fss-0.4.3/dart_fss/tests/test_corp.py
+-rw-rw-rw-   0        0        0     1004 2023-03-31 07:24:27.000000 dart-fss-0.4.3/dart_fss/tests/test_errors.py
+-rw-rw-rw-   0        0        0     4456 2023-04-24 05:50:55.000000 dart-fss-0.4.3/dart_fss/tests/test_fs.py
+-rw-rw-rw-   0        0        0      775 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_fs_search.py
+-rw-rw-rw-   0        0        0      469 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_regex.py
+-rw-rw-rw-   0        0        0     1320 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_reports.py
+-rw-rw-rw-   0        0        0      804 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_search_report.py
+-rw-rw-rw-   0        0        0      653 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_utils.py
+-rw-rw-rw-   0        0        0     2706 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/tests/test_xbrl.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.358605 dart-fss-0.4.3/dart_fss/utils/
+-rw-rw-rw-   0        0        0     1277 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/cache.py
+-rw-rw-rw-   0        0        0      704 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/dataframe.py
+-rw-rw-rw-   0        0        0     1434 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/datetime.py
+-rw-rw-rw-   0        0        0     2666 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/file.py
+-rw-rw-rw-   0        0        0     2733 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/notebook.py
+-rw-rw-rw-   0        0        0     3077 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/regex.py
+-rw-rw-rw-   0        0        0     7602 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/request.py
+-rw-rw-rw-   0        0        0      304 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/singleton.py
+-rw-rw-rw-   0        0        0     1019 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/spinner.py
+-rw-rw-rw-   0        0        0     2134 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/utils/string.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:23.374163 dart-fss-0.4.3/dart_fss/xbrl/
+-rw-rw-rw-   0        0        0       97 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/__init__.py
+-rw-rw-rw-   0        0        0    10993 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/dart_xbrl.py
+-rw-rw-rw-   0        0        0    12749 2023-03-06 00:18:03.000000 dart-fss-0.4.3/dart_fss/xbrl/helper.py
+-rw-rw-rw-   0        0        0     9229 2023-03-31 07:17:35.000000 dart-fss-0.4.3/dart_fss/xbrl/table.py
+-rw-rw-rw-   0        0        0     1441 2023-03-07 00:46:47.000000 dart-fss-0.4.3/dart_fss/xbrl/xbrl.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:35:22.885001 dart-fss-0.4.3/dart_fss.egg-info/
+-rw-rw-rw-   0        0        0     3289 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5450 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 00:35:22.000000 dart-fss-0.4.3/dart_fss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1162 2023-04-25 00:34:38.000000 dart-fss-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0      108 2023-04-24 05:30:51.000000 dart-fss-0.4.3/requirements.txt
+-rw-rw-rw-   0        0        0      186 2023-04-25 00:35:23.377140 dart-fss-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-04-24 04:56:16.000000 dart-fss-0.4.3/setup.py
+-rw-rw-rw-   0        0        0    85812 2023-04-24 02:48:24.000000 dart-fss-0.4.3/versioneer.py
```

### Comparing `dart-fss-0.4.2/LICENSE` & `dart-fss-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/PKG-INFO` & `dart-fss-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dart-fss
-Version: 0.4.2
+Version: 0.4.3
 Summary: Web-scraping https://dart.fss.or.kr
-Home-page: https://github.com/josw123/dart-fss
-Author: Sungwoo Jo
-Author-email: nonswing.z@gmail.com
+Author-email: Sungwoo Jo <nonswing.z@gmail.com>
+Maintainer-email: Sungwoo Jo <nonswing.z@gmail.com>
 License: MIT
-Keywords: fss,dart-fss,scrapping
+Project-URL: homepage, https://github.com/josw123/dart-fss
+Project-URL: documentation, https://dart-fss.readthedocs.io/
+Project-URL: repository, https://github.com/josw123/dart-fss.git
+Keywords: fss,dart-fss,scrapping,financial statement
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 License-File: LICENSE
 
 # Dart-Fss
 [![PyPI](https://img.shields.io/pypi/v/dart-fss.svg)](https://pypi.org/project/dart-fss/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dart-fss.svg)
 ![Build Status](https://bit.ly/3fufevG)
 [![Coverage](https://codecov.io/gh/josw123/dart-fss/branch/master/graphs/badge.svg)](https://codecov.io/gh/josw123/dart-fss)
```

### Comparing `dart-fss-0.4.2/README.md` & `dart-fss-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/__init__.py` & `dart-fss-0.4.3/dart_fss/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/_version.py` & `dart-fss-0.4.3/dart_fss/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-# This file was generated by 'versioneer.py' (0.20) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-03-07T19:55:34+0900",
+ "date": "2023-04-25T09:31:43+0900",
  "dirty": false,
  "error": null,
- "full-revisionid": "2c650cdbeac40c724737d90749c0097ec1a46809",
- "version": "0.4.2"
+ "full-revisionid": "3a8f0b92ad00f7bf811bd0f6549ad06ee9084f9e",
+ "version": "0.4.3"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `dart-fss-0.4.2/dart_fss/api/filings/corp_code.py` & `dart-fss-0.4.3/dart_fss/api/filings/corp_code.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/filings/document.py` & `dart-fss-0.4.3/dart_fss/api/filings/document.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/filings/search_filings.py` & `dart-fss-0.4.3/dart_fss/api/filings/search_filings.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/finance/fnltt_multi_acnt.py` & `dart-fss-0.4.3/dart_fss/api/finance/fnltt_multi_acnt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/finance/fnltt_singl_acnt.py` & `dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/finance/fnltt_singl_acnt_all.py` & `dart-fss-0.4.3/dart_fss/api/finance/fnltt_singl_acnt_all.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/finance/xbrl.py` & `dart-fss-0.4.3/dart_fss/api/finance/xbrl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/finance/xbrl_taxonomy.py` & `dart-fss-0.4.3/dart_fss/api/finance/xbrl_taxonomy.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/helper.py` & `dart-fss-0.4.3/dart_fss/api/helper.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/__init__.py` & `dart-fss-0.4.3/dart_fss/api/info/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py` & `dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_nm_nd_adt_opinion.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/accnut_adtor_non_adt_servc_cncls_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/adt_servc_cncls_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/adt_servc_cncls_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/alot_matter.py` & `dart-fss-0.4.3/dart_fss/api/info/alot_matter.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py` & `dart-fss-0.4.3/dart_fss/api/info/cndl_capl_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/cprnd_nrdmp_blce.py` & `dart-fss-0.4.3/dart_fss/api/info/cprnd_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/det_scrits_isu_acmslt.py` & `dart-fss-0.4.3/dart_fss/api/info/det_scrits_isu_acmslt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py` & `dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_gmtsck_confm_amount.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py` & `dart-fss-0.4.3/dart_fss/api/info/drctr_adt_all_mendng_sttus_mendng_pymntamt_ty_cl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/emp_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/emp_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py` & `dart-fss-0.4.3/dart_fss/api/info/entrprs_bil_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/exctv_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/exctv_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/hmv_audit_all_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/hmv_audit_all_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/hmv_audit_indvdl_by_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/hyslr_chg_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/hyslr_chg_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/hyslr_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/hyslr_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/indvdl_by_pay.py` & `dart-fss-0.4.3/dart_fss/api/info/indvdl_by_pay.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/irds_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/irds_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/mrhl_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/mrhl_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py` & `dart-fss-0.4.3/dart_fss/api/info/new_capl_scrits_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/otr_cpr_invstmnt_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/otr_cpr_invstmnt_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/outcmpny_drctr_nd_change_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/prvsrp_cptal_use_dtls.py` & `dart-fss-0.4.3/dart_fss/api/info/prvsrp_cptal_use_dtls.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/pssrp_cptal_use_dtls.py` & `dart-fss-0.4.3/dart_fss/api/info/pssrp_cptal_use_dtls.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py` & `dart-fss-0.4.3/dart_fss/api/info/srtpd_psndbt_nrdmp_blce.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/stock_totqy_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/stock_totqy_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/tesstk_acqs_dsps_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/tesstk_acqs_dsps_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/info/unrst_exctv_mendng_sttus.py` & `dart-fss-0.4.3/dart_fss/api/info/unrst_exctv_mendng_sttus.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/__init__.py` & `dart-fss-0.4.3/dart_fss/api/issue/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py` & `dart-fss-0.4.3/dart_fss/api/issue/ast_inhtrf_etc_ptbk_opt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bdwt_is_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/bdwt_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bnk_mngt_pcbg.py` & `dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcbg.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bnk_mngt_pcsp.py` & `dart-fss-0.4.3/dart_fss/api/issue/bnk_mngt_pcsp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bsn_inh_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/bsn_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bsn_sp.py` & `dart-fss-0.4.3/dart_fss/api/issue/bsn_sp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/bsn_trf_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/bsn_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/cmp_dv_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/cmp_dv_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/cmp_dvmg_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/cmp_dvmg_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/cmp_mg_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/cmp_mg_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/cr_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/cr_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ctrcvs_bgrq.py` & `dart-fss-0.4.3/dart_fss/api/issue/ctrcvs_bgrq.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/cvbd_is_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/cvbd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/df_ocr.py` & `dart-fss-0.4.3/dart_fss/api/issue/df_ocr.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ds_rs_ocr.py` & `dart-fss-0.4.3/dart_fss/api/issue/ds_rs_ocr.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/exbd_is_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/exbd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/fric_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/fric_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/lwst_lg.py` & `dart-fss-0.4.3/dart_fss/api/issue/lwst_lg.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/otcpr_stk_invscr_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ov_dlst.py` & `dart-fss-0.4.3/dart_fss/api/issue/ov_dlst.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ov_dlst_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/ov_dlst_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ov_lst.py` & `dart-fss-0.4.3/dart_fss/api/issue/ov_lst.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/ov_lst_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/ov_lst_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/pifric_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/pifric_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/piic_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/piic_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/stk_extr_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/stk_extr_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/stkrtbd_inh_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/stkrtbd_trf_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/stkrtbd_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tgast_inh_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tgast_inh_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tgast_trf_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tgast_trf_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cc_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tsstk_aq_trctr_cns_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/tsstk_dp_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/tsstk_dp_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/issue/wd_cocobd_is_decsn.py` & `dart-fss-0.4.3/dart_fss/api/issue/wd_cocobd_is_decsn.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/market/stock_market.py` & `dart-fss-0.4.3/dart_fss/api/market/stock_market.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/market/trading_halt.py` & `dart-fss-0.4.3/dart_fss/api/market/trading_halt.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/bd_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/bd_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/dv_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/dv_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/estk_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/estk_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/extr_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/extr_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/mg_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/mg_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/registration/stkdp_rs.py` & `dart-fss-0.4.3/dart_fss/api/registration/stkdp_rs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/shareholder/elestock.py` & `dart-fss-0.4.3/dart_fss/api/shareholder/elestock.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/api/shareholder/majorstock.py` & `dart-fss-0.4.3/dart_fss/api/shareholder/majorstock.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/auth/auth.py` & `dart-fss-0.4.3/dart_fss/auth/auth.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/corp/corp.py` & `dart-fss-0.4.3/dart_fss/corp/corp.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/corp/corp_list.py` & `dart-fss-0.4.3/dart_fss/corp/corp_list.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/errors/checker.py` & `dart-fss-0.4.3/dart_fss/errors/checker.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/errors/errors.py` & `dart-fss-0.4.3/dart_fss/errors/errors.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/filings/pages.py` & `dart-fss-0.4.3/dart_fss/filings/pages.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/filings/reports.py` & `dart-fss-0.4.3/dart_fss/filings/reports.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/filings/search.py` & `dart-fss-0.4.3/dart_fss/filings/search.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/filings/search_result.py` & `dart-fss-0.4.3/dart_fss/filings/search_result.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/fs/extract.py` & `dart-fss-0.4.3/dart_fss/fs/extract.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/fs/fs.py` & `dart-fss-0.4.3/dart_fss/fs/fs.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/__init__.py` & `dart-fss-0.4.3/dart_fss/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/cache.py` & `dart-fss-0.4.3/dart_fss/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/dataframe.py` & `dart-fss-0.4.3/dart_fss/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/datetime.py` & `dart-fss-0.4.3/dart_fss/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/file.py` & `dart-fss-0.4.3/dart_fss/utils/file.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/notebook.py` & `dart-fss-0.4.3/dart_fss/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/regex.py` & `dart-fss-0.4.3/dart_fss/utils/regex.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/request.py` & `dart-fss-0.4.3/dart_fss/utils/request.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/spinner.py` & `dart-fss-0.4.3/dart_fss/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/utils/string.py` & `dart-fss-0.4.3/dart_fss/utils/string.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/xbrl/dart_xbrl.py` & `dart-fss-0.4.3/dart_fss/xbrl/dart_xbrl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/xbrl/helper.py` & `dart-fss-0.4.3/dart_fss/xbrl/helper.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss/xbrl/table.py` & `dart-fss-0.4.3/dart_fss/xbrl/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,20 +146,20 @@
         self._cls = cls
         return self._cls
 
     @property
     def labels(self):
         """labels 반환"""
         if self._labels is None:
-            self._labels = {}
+            self._labels = []
             arcrole = XbrlConst.parentChild
             relationship_set = self._xbrl.relationshipSet(arcrole, self.uri)
             for root_concept in relationship_set.rootConcepts:
                 labels = get_label_list(relationship_set, root_concept)
-                self._labels = {**self._labels, **labels}
+                self._labels.append(labels)
         return self._labels
 
     def to_DataFrame(self, cls=None, lang='ko', start_dt=None, end_dt=None,
                      label=None, show_abstract=False, show_class=True, show_depth=10,
                      show_concept=True, separator=True):
         """ Pandas DataFrame으로 변환하는 함수
 
@@ -190,15 +190,18 @@
         -------
         DataFrame
             재무제표 DataFrame
         """
         if cls is None:
             cls = self.cls_filter(start_dt, end_dt, label)
         cls = cls_merge_type(cls)
-        depth = get_max_depth(self.labels, show_abstract=show_abstract)
+
+        depth = -1
+        for label in self.labels:
+            depth = max(depth, get_max_depth(label, show_abstract=show_abstract))
         depth = depth if depth < show_depth else show_depth
 
         table = self.parent.get_table_by_code('d999004')
         unit = get_value_from_dataset(table.cls, table.dataset, 'dart-gcd_EntityReportingCurrencyISOCode')
 
         definition = self.definition + ' (Unit: {})'.format(unit[0])
         columns = generate_df_columns(definition, cls, depth, lang,
@@ -206,16 +209,20 @@
 
         if separator:
             pd.options.display.float_format = '{:,}'.format
         else:
             pd.options.display.float_format = '{:}'.format
         df = pd.DataFrame(columns=columns)
 
-        rows = generate_df_rows(self.labels, cls, self.dataset, depth, lang=lang,
+        rows = []
+        for label in self.labels:
+            r = generate_df_rows(label, cls, self.dataset, depth, lang=lang,
                                 show_abstract=show_abstract, show_concept=show_concept, show_class=show_class)
+            rows.append(r)
+        rows = flatten(rows)
         data = flatten(rows)
         for idx, r in enumerate(data):
             df.loc[idx] = r
 
         regex_pass = str_to_regex('concept_id OR label_ko OR label_en OR class')
         df_count = df.count()
         drop_columns = []
```

### Comparing `dart-fss-0.4.2/dart_fss/xbrl/xbrl.py` & `dart-fss-0.4.3/dart_fss/xbrl/xbrl.py`

 * *Files identical despite different names*

### Comparing `dart-fss-0.4.2/dart_fss.egg-info/PKG-INFO` & `dart-fss-0.4.3/dart_fss.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dart-fss
-Version: 0.4.2
+Version: 0.4.3
 Summary: Web-scraping https://dart.fss.or.kr
-Home-page: https://github.com/josw123/dart-fss
-Author: Sungwoo Jo
-Author-email: nonswing.z@gmail.com
+Author-email: Sungwoo Jo <nonswing.z@gmail.com>
+Maintainer-email: Sungwoo Jo <nonswing.z@gmail.com>
 License: MIT
-Keywords: fss,dart-fss,scrapping
+Project-URL: homepage, https://github.com/josw123/dart-fss
+Project-URL: documentation, https://dart-fss.readthedocs.io/
+Project-URL: repository, https://github.com/josw123/dart-fss.git
+Keywords: fss,dart-fss,scrapping,financial statement
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 License-File: LICENSE
 
 # Dart-Fss
 [![PyPI](https://img.shields.io/pypi/v/dart-fss.svg)](https://pypi.org/project/dart-fss/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dart-fss.svg)
 ![Build Status](https://bit.ly/3fufevG)
 [![Coverage](https://codecov.io/gh/josw123/dart-fss/branch/master/graphs/badge.svg)](https://codecov.io/gh/josw123/dart-fss)
```

### Comparing `dart-fss-0.4.2/versioneer.py` & `dart-fss-0.4.3/versioneer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 
-# Version: 0.20
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -227,17 +255,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -259,36 +288,52 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable, Dict
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods # noqa
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
@@ -315,85 +360,101 @@
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
                   % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
 
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+        section = parser["versioneer"]
 
-    # pylint:disable=attribute-defined-outside-init # noqa
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
+    cfg.VCS = section['VCS']
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
     cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
@@ -413,24 +474,27 @@
 LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.20 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Callable, Dict
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -438,15 +502,15 @@
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
     git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_config():
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
@@ -460,45 +524,52 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
@@ -558,15 +629,15 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
@@ -639,27 +710,34 @@
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match", "%%s*" %% tag_prefix],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -715,15 +793,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -740,16 +818,16 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
@@ -815,24 +893,42 @@
         rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
 def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
@@ -1055,15 +1151,15 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
@@ -1136,27 +1232,34 @@
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match", "%s*" % tag_prefix],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1212,15 +1315,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1237,56 +1340,57 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
                         break
-    except EnvironmentError:
+    except OSError:
         pass
     if not present:
         with open(".gitattributes", "a+") as fobj:
             fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
@@ -1312,15 +1416,15 @@
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.20) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1334,15 +1438,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1419,24 +1523,42 @@
         rendered += "+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
 def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
@@ -1675,15 +1797,15 @@
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
 def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
+    """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1697,16 +1819,16 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1721,58 +1843,61 @@
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if 'build_py' in cmds:
         _build_py = cmds['build_py']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
     if 'build_ext' in cmds:
         _build_ext = cmds['build_ext']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_ext import build_ext as _build_ext
     else:
-        from distutils.command.build_ext import build_ext as _build_ext
+        from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
@@ -1780,16 +1905,23 @@
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
+            if not cfg.versionfile_build:
+                return
             target_versionfile = os.path.join(self.build_lib,
                                               cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
@@ -1819,15 +1951,18 @@
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1843,26 +1978,60 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if 'sdist' in cmds:
         _sdist = cmds['sdist']
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
-            # pylint:disable=attribute-defined-outside-init # noqa
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
         def make_release_tree(self, base_dir, files):
@@ -1931,17 +2100,17 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1957,15 +2126,15 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
             print(" replacing boilerplate in %s" % ipy)
             with open(ipy, "w") as f:
                 f.write(old.replace(OLD_SNIPPET, snippet))
@@ -1975,50 +2144,18 @@
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -2051,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```


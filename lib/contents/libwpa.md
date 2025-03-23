```sh
xtensa-lx106-elf-nm --defined-only libwpa.a | less
```

ap_config.o:
00000020 T hostapd_config_defaults
00000008 T hostapd_config_defaults_bss
00000004 T hostapd_get_psk
00000004 T hostapd_mac_comp
00000008 T hostapd_mac_comp_empty
00000004 T hostapd_maclist_found
00000000 T hostapd_rate_found
00000004 T hostapd_setup_wpa_psk
00000004 T hostapd_wep_key_cmp

common.o:
0000000c T dup_binstr
00000008 T hex2byte
00000004 T hexstr2bin
00000000 T inc_byte_array
00000034 T wpa_config_parse_string
0000001c T wpa_get_ntp_timestamp

ieee802_1x.o:
00000008 T ieee802_1x_receive

os_xtensa.o:
00000010 T ets_strdup
00000004 T os_get_random
00000000 T os_get_time
00000004 T os_random
00000004 T r_rand

sta_info.o:

wpa_auth.o:
000000ac T __wpa_send_eapol
00000004 B resend_eapol
00000008 T resend_eapol_handle
00000000 T wpa_auth_for_each_sta
00000010 T wpa_auth_sm_event
00000010 T wpa_auth_sta_associated
00000004 T wpa_auth_sta_deinit
00000010 T wpa_auth_sta_init
00000000 T wpa_auth_sta_no_wpa
00000030 T wpa_init
00000094 T wpa_receive
00000010 T wpa_remove_ptk

wpa_auth_ie.o:
00000008 T wpa_add_kde
0000001c T wpa_auth_gen_wpa_ie
00000000 T wpa_auth_uses_mfp
00000008 T wpa_parse_kde_ies
00000028 T wpa_validate_wpa_ie
0000000c T wpa_write_rsn_ie

wpabuf.o:
00000008 T wpabuf_alloc
00000008 T wpabuf_alloc_copy
00000008 T wpabuf_alloc_ext_data
00000014 T wpabuf_concat
00000008 T wpabuf_dup
00000010 T wpabuf_free
0000000c T wpabuf_printf
00000008 T wpabuf_put
00000018 T wpabuf_resize
00000014 T wpabuf_zeropad

wpa.o:
00000018 T eapol_txcb
00000058 T pp_michael_mic_failure
00000008 T wpa_register
00000034 T wpa_set_bss
0000000c T wpa_set_pmk
00000004 T wpa_set_profile
00000028 T wpa_sm_rx_eapol
00000010 T wpa_sm_set_state

wpa_common.o:
00000000 T rsn_cipher_put_suites
00000014 T rsn_pmkid
00000000 T wpa_cipher_key_len
00000000 T wpa_cipher_put_suites
00000000 T wpa_cipher_to_alg
0000002c T wpa_cipher_to_suite
00000004 T wpa_compare_rsn_ie
0000000c T wpa_eapol_key_mic
00000010 T wpa_parse_wpa_ie_rsn
00000014 T wpa_parse_wpa_ie_wpa
0000002c T wpa_pmk_to_ptk

wpa_debug.o:
00000000 T eloop_cancel_timeout
00000000 T eloop_register_timeout
00000004 T wpa_snprintf_hex
00000004 T wpa_snprintf_hex_uppercase

wpa_ie.o:
00000008 T wpa_gen_wpa_ie
00000008 T wpa_parse_wpa_ie
00000008 T wpa_supplicant_parse_ies

wpa_main.o:
00000008 T dhcp_bind_check
0000009c T eagle_auth_done
00000004 T ppGetKey
00000048 T ppInstallKey
00000024 T wpa_attach
00000004 T wpa_config_assoc_ie
00000004 T wpa_config_bss
00000008 T wpa_config_profile
00000004 T wpa_neg_complete

wpas_glue.o:
00000008 T wpa_sm_alloc_eapol
00000000 T wpa_sm_deauthenticate
00000000 T wpa_sm_disassociate
00000000 T wpa_sm_get_beacon_ie
00000000 T wpa_sm_mlme_setprotection

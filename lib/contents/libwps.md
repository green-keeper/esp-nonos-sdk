```sh
xtensa-lx106-elf-nm --defined-only libwps.a | less
```

eap_common.o:
00000004 T eap_get_id
00000004 T eap_get_type
00000004 T eap_hdr_len_valid
00000008 T eap_hdr_validate
00000018 T eap_msg_alloc
00000000 T eap_update_len

uuid.o:
00000000 T is_nil_uuid
00000008 T uuid_bin2str
00000014 T uuid_str2bin

wps_attr_build.o:
00000010 T wps_build_assoc_state
00000010 T wps_build_auth_type_flags
0000001c T wps_build_authenticator
00000010 T wps_build_config_error
00000010 T wps_build_config_methods
00000010 T wps_build_conn_type_flags
00000010 T wps_build_dev_password_id
00000028 T wps_build_encr_settings
00000010 T wps_build_encr_type_flags
00000010 T wps_build_enrollee_nonce
00000018 T wps_build_key_wrap_auth
00000010 T wps_build_msg_type
0000005c T wps_build_public_key
00000010 T wps_build_registrar_nonce
00000010 T wps_build_req_type
00000010 T wps_build_resp_type
00000010 T wps_build_uuid_e
00000010 T wps_build_version
00000040 T wps_build_wfa_ext
00000028 T wps_ie_encapsulate

wps_attr_parse.o:
00000008 T wps_parse_msg

wps_attr_process.o:
00000020 T wps_process_ap_settings
00000008 T wps_process_authenticator
00000034 T wps_process_cred
00000008 T wps_process_key_wrap_auth

wps.o:
00000000 T show_buf
0000000c T wifi_set_wps_cb
00000048 T wifi_station_wps_deinit
000000ac T wifi_station_wps_init
00000020 T wifi_station_wps_start
00000004 T wifi_station_wps_success
00000010 T wifi_station_wps_timeout
00000030 T wifi_wps_disable
00000024 T wifi_wps_enable
0000000c T wifi_wps_scan
0000000c T wifi_wps_scan_done
00000020 T wifi_wps_start
00000008 T wps_ap_priority_compar
00000060 T wps_attr_text
00000024 T wps_build_assoc_req_ie
00000024 T wps_build_assoc_resp_ie
0000004c T wps_build_probe_req_ie
0000002c T wps_deinit
00000018 T wps_dev_deinit
00000060 T wps_dev_init
00000008 T wps_get_msg
00000004 T wps_get_uuid_e
0000005c T wps_init
00000004 T wps_is_20
0000001c T wps_is_addr_authorized
0000001c T wps_is_selected_pbc_registrar
00000008 T wps_is_selected_pin_registrar
00000028 T wps_key_save
00000008 T wps_process_msg
00000014 T wps_process_wps_mX_req
00000024 T wps_send_eap_identity_rsp
0000003c T wps_send_wps_mX_rsp
00000008 T wps_sm_alloc_eapol
00000004 T wps_sm_get
00000078 T wps_sm_rx_eapol
00000008 T wps_start_pending
00000004 T wps_station_wps_register_cb
00000018 T wps_txStart

wps_common.o:
00000010 T uuid_gen_mac_addr
0000001c T wps_build_wsc_ack
00000020 T wps_build_wsc_nack
0000006c T wps_config_methods_str2bin
0000001c T wps_decrypt_encr_settings
00000030 T wps_derive_keys
00000010 T wps_derive_psk
00000008 T wps_dev_type_bin2str
0000001c T wps_dev_type_str2bin
00000004 T wps_fail_event
00000014 T wps_generate_pin
00000010 T wps_kdf
00000000 T wps_pbc_overlap_event
00000000 T wps_pbc_timeout_event
00000018 T wps_pin_checksum
00000000 T wps_pin_str_valid
0000000c T wps_pin_valid
00000004 T wps_pwd_auth_fail_event
00000000 T wps_success_event

wps_dev_attr.o:
00000014 T wps_build_dev_name
00000018 T wps_build_device_attrs
00000014 T wps_build_manufacturer
00000014 T wps_build_model_name
00000014 T wps_build_model_number
00000014 T wps_build_os_version
00000010 T wps_build_primary_dev_type
00000010 T wps_build_req_dev_type
00000010 T wps_build_rf_bands
00000010 T wps_build_secondary_dev_type
00000014 T wps_build_vendor_ext
00000014 T wps_build_vendor_ext_m1
00000018 T wps_device_data_dup
00000018 T wps_device_data_free
00000018 T wps_process_device_attrs
00000000 T wps_process_os_version
00000000 T wps_process_rf_bands

wps_enrollee.o:
00000028 T wps_enrollee_get_msg
0000001c T wps_enrollee_process_msg

wps_registrar.o:
00000000 T wps_authorized_macs
00000070 T wps_build_cred
00000020 T wps_build_credential_wrap
00000014 T wps_device_store
0000003c T wps_registrar_add_pin
00000034 T wps_registrar_button_pushed
00000018 T wps_registrar_complete
00000000 T wps_registrar_config_ap
00000028 T wps_registrar_deinit
00000028 T wps_registrar_get_info
0000002c T wps_registrar_get_msg
0000001c T wps_registrar_init
00000008 T wps_registrar_invalidate_pin
0000000c T wps_registrar_pbc_overlap
00000024 T wps_registrar_probe_req_rx
00000020 T wps_registrar_process_msg
0000001c T wps_registrar_selected_registrar_changed
00000008 T wps_registrar_unlock_pin
00000004 T wps_registrar_update_ie
00000014 T wps_registrar_wps_cancel

wps_validate.o:
00000010 T wps_validate_assoc_req
00000010 T wps_validate_assoc_resp
0000002c T wps_validate_beacon
0000004c T wps_validate_beacon_probe_resp
00000064 T wps_validate_m1
00000060 T wps_validate_m2
00000054 T wps_validate_m2d
00000020 T wps_validate_m3
00000024 T wps_validate_m4
0000000c T wps_validate_m4_encr
0000001c T wps_validate_m5
0000000c T wps_validate_m5_encr
0000001c T wps_validate_m6
0000000c T wps_validate_m6_encr
00000020 T wps_validate_m7
00000024 T wps_validate_m7_encr
0000001c T wps_validate_m8
00000020 T wps_validate_m8_encr
00000048 T wps_validate_probe_req
0000001c T wps_validate_upnp_set_selected_registrar
00000018 T wps_validate_wsc_ack
00000018 T wps_validate_wsc_done
0000001c T wps_validate_wsc_nack

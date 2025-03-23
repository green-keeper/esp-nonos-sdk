```sh
xtensa-lx106-elf-nm --defined-only libcrypto.a | less
```

aes-cbc.o:
00000018 T aes_128_cbc_decrypt
00000014 T aes_128_cbc_encrypt

aes-internal.o:
0000001c T rijndaelKeySetupEnc

aes-internal-dec.o:
00000004 T aes_decrypt
0000000c T aes_decrypt_deinit
00000014 T aes_decrypt_init

aes-internal-enc.o:
00000004 T aes_encrypt
0000000c T aes_encrypt_deinit
00000014 T aes_encrypt_init
00000010 T rijndaelEncrypt

aes-wrap.o:
00000024 T aes_wrap

bignum.o:
00000004 T bignum_add
00000004 T bignum_cmp
00000004 T bignum_cmp_d
0000000c T bignum_deinit
00000004 T bignum_exptmod
00000008 T bignum_get_unsigned_bin
00000004 T bignum_get_unsigned_bin_len
00000014 T bignum_init
00000004 T bignum_mul
00000004 T bignum_mulmod
00000004 T bignum_set_unsigned_bin
00000004 T bignum_sub

crypto_internal.o:
00000000 T crypto_global_deinit
00000000 T crypto_global_init
00000088 T crypto_hash_finish
00000078 T crypto_hash_init
0000000c T crypto_hash_update

crypto_internal-cipher.o:
00000014 T crypto_cipher_decrypt
00000010 T crypto_cipher_deinit
00000010 T crypto_cipher_encrypt
0000003c T crypto_cipher_init

crypto_internal-modexp.o:
00000034 T crypto_mod_exp

crypto_internal-rsa.o:
00000004 T crypto_private_key_decrypt_pkcs1_v15
00000004 T crypto_private_key_free
0000000c T crypto_private_key_import
00000004 T crypto_private_key_sign_pkcs1
00000004 T crypto_public_key_decrypt_pkcs1
00000004 T crypto_public_key_encrypt_pkcs1_v15
00000004 T crypto_public_key_free
00000000 T crypto_public_key_from_cert
00000004 T crypto_public_key_import

des-internal.o:
00000010 T des_encrypt

dh_group5.o:
00000008 T dh5_derive_shared
00000000 T dh5_free
00000008 T dh5_init

dh_groups.o:
00000018 T dh_derive_shared
00000004 T dh_groups_get
00000030 T dh_init

md4-internal.o:
0000000c T md4_vector

ms_funcs.o:
00000010 T challenge_response
00000014 T encrypt_pw_block_with_password_hash
00000008 T generate_authenticator_response
00000014 T generate_authenticator_response_pwhash
0000000c T generate_nt_response
00000008 T generate_nt_response_pwhash
0000001c T get_asymetric_start_key
0000000c T get_master_key
00000004 T hash_nt_password_hash
00000008 T new_password_encrypted_with_old_nt_password_hash
00000008 T nt_challenge_response
00000008 T nt_password_hash
00000008 T nt_password_hash_encrypted_with_block
0000000c T old_nt_password_hash_encrypted_with_new_nt_password_hash

sha256.o:
00000004 T hmac_sha256
0000001c T hmac_sha256_vector
00000010 T sha256_prf

sha256-internal.o:
00000008 T sha256_done
00000020 T sha256_init
0000000c T sha256_process
0000000c T sha256_vector


idf_component_register(SRCS "app/src/app_mqtt_code.c" 
                            "oneNET_token/initialToken.c"
                            "oneNET_token/cipher/hmac.c"
                            "oneNET_token/cipher/md5.c"
                           "oneNET_token/cipher/sha1.c"
                            "oneNET_token/cipher/sha256.c"
                    INCLUDE_DIRS "app/include" "oneNET_token" "oneNET_token/cipher"
                    REQUIRES mbedtls nvs_flash protocol_examples_common mqtt 
                     )


idf_component_register(SRCS "main.c" 
                            "../componnects/app/src/app_mqtt_code.c" 
                            "../componnects/oneNET_token/cipher/hmac.c"
                            "../componnects/oneNET_token/cipher/md5.c"
                             "../componnects/oneNET_token/cipher/sha.c"
                            "../componnects/oneNET_token/cipher/sha1.c"
                            "../componnects/oneNET_token/cipher/sha256.c"
                            "../componnects/oneNET_token/initialToken.c"

                    INCLUDE_DIRS "."  "../componnects/app/include" "../componnects/oneNET_token" "../componnects/oneNET_token/cipher"
                    REQUIRES mbedtls nvs_flash protocol_examples_common mqtt pthread
                    )

cmake_minimum_required(VERSION 3.4.1)
aux_source_directory(. playfair_src)
set(playfair_src ${playfair_src})
list(APPEND playfair_src
        hand_garble.c
        modified_md5.c
        omg_hax.c
        playfair.c
        sap_hash.c
)
add_library( playfair
        STATIC
        ${playfair_src})
if GCRYPT
gcrypt_needing_programs = tomb-kdf-pbkdf2 tomb-kdf-pbkdf2-getiter
else
gcrypt_needing_programs=
endif
	

bin_PROGRAMS = $(gcrypt_needing_programs) tomb-kdf-pbkdf2-gensalt hexencode
tomb_kdf_pbkdf2_SOURCES = pbkdf2/pbkdf2.c
tomb_kdf_pbkdf2_CFLAGS = $(LIBGCRYPT_CFLAGS)
tomb_kdf_pbkdf2_LDADD = $(LIBGCRYPT_LIBS)

tomb_kdf_pbkdf2_gensalt_SOURCES = pbkdf2/gen_salt.c

tomb_kdf_pbkdf2_getiter_SOURCES = pbkdf2/benchmark.c
tomb_kdf_pbkdf2_getiter_CFLAGS = $(LIBGCRYPT_CFLAGS)
tomb_kdf_pbkdf2_getiter_LDADD = $(LIBGCRYPT_LIBS)

hexencode_SOURCES = hexencode.c


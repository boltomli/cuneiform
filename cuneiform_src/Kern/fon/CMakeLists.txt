add_library(fon32 ${LIBTYPE}
src/clu_best.c
src/clu_div.c
src/clu_lang.c
src/clu_test.c
src/cutoff.c
src/dist_bou.c
src/distance.c
src/fon_snap.c
src/fonrec.c
src/p2_addcl.c
src/p2_clu.c
src/p2_dsbit.c
src/p2_mem.c
src/p2_thick.c
src/utilctb.c
)
set_property(TARGET fon32 PROPERTY COMPILE_DEFINITIONS __FON__)

target_link_libraries(fon32 cstr ctb32)

library_hook(fon32)

PLATFORM=$(shell uname|tr A-Z a-z)

CC				= gcc
CXX				= g++
B					= Build
INST				= Install
BASE    		= Base
JAMPG    		= jampgamei386
OPENJKDED   = openjkded.i386
LIB 				= lib

DLL_EXT		= so

GAME_NAME			= $(B)/$(INST)/$(BASE)/jampgamei386.$(DLL_EXT)
GAME_CFLAGS		= -msse2 -Wall -Wno-comment -fvisibility=hidden -fsigned-char -mstackrealign -mfpmath=sse -O2 -DNDEBUG -O2 -fPIC -I.
GAME_CDEFINES	= -DARCH_STRING=\"i386\" -DFINAL_BUILD -D_GAME -Djampgamei386_EXPORTS
GAME_LDFLAGS		= -m32 -shared -lm
GAME_OBJS			=	$(B)/$(JAMPG)/game/ai_main.o \
								$(B)/$(JAMPG)/game/ai_util.o \
								$(B)/$(JAMPG)/game/ai_wpnav.o \
								$(B)/$(JAMPG)/game/AnimalNPC.o \
								$(B)/$(JAMPG)/game/bg_g2_utils.o \
								$(B)/$(JAMPG)/game/bg_misc.o \
								$(B)/$(JAMPG)/game/bg_panimate.o \
								$(B)/$(JAMPG)/game/bg_pmove.o \
								$(B)/$(JAMPG)/game/bg_saber.o \
								$(B)/$(JAMPG)/game/bg_saberLoad.o \
								$(B)/$(JAMPG)/game/bg_saga.o \
								$(B)/$(JAMPG)/game/bg_slidemove.o \
								$(B)/$(JAMPG)/game/bg_vehicleLoad.o \
								$(B)/$(JAMPG)/game/bg_weapons.o \
								$(B)/$(JAMPG)/game/FighterNPC.o \
								$(B)/$(JAMPG)/game/g_active.o \
								$(B)/$(JAMPG)/game/g_bot.o \
								$(B)/$(JAMPG)/game/g_client.o \
								$(B)/$(JAMPG)/game/g_cmds.o \
								$(B)/$(JAMPG)/game/g_combat.o \
								$(B)/$(JAMPG)/game/g_cvar.o \
								$(B)/$(JAMPG)/game/g_exphysics.o \
								$(B)/$(JAMPG)/game/g_ICARUScb.o \
								$(B)/$(JAMPG)/game/g_items.o \
								$(B)/$(JAMPG)/game/g_log.o \
								$(B)/$(JAMPG)/game/g_main.o \
								$(B)/$(JAMPG)/game/g_mem.o \
								$(B)/$(JAMPG)/game/g_misc.o \
								$(B)/$(JAMPG)/game/g_missile.o \
								$(B)/$(JAMPG)/game/g_mover.o \
								$(B)/$(JAMPG)/game/g_nav.o \
								$(B)/$(JAMPG)/game/g_navnew.o \
								$(B)/$(JAMPG)/game/g_object.o \
								$(B)/$(JAMPG)/game/g_saga.o \
								$(B)/$(JAMPG)/game/g_session.o \
								$(B)/$(JAMPG)/game/g_spawn.o \
								$(B)/$(JAMPG)/game/g_svcmds.o \
								$(B)/$(JAMPG)/game/g_syscalls.o \
								$(B)/$(JAMPG)/game/g_target.o \
								$(B)/$(JAMPG)/game/g_team.o \
								$(B)/$(JAMPG)/game/g_timer.o \
								$(B)/$(JAMPG)/game/g_trigger.o \
								$(B)/$(JAMPG)/game/g_turret_G2.o \
								$(B)/$(JAMPG)/game/g_turret.o \
								$(B)/$(JAMPG)/game/g_utils.o \
								$(B)/$(JAMPG)/game/g_vehicles.o \
								$(B)/$(JAMPG)/game/g_vehicleTurret.o \
								$(B)/$(JAMPG)/game/g_weapon.o \
								$(B)/$(JAMPG)/game/NPC_AI_Atst.o \
								$(B)/$(JAMPG)/game/NPC_AI_Default.o \
								$(B)/$(JAMPG)/game/NPC_AI_Droid.o \
								$(B)/$(JAMPG)/game/NPC_AI_GalakMech.o \
								$(B)/$(JAMPG)/game/NPC_AI_Grenadier.o \
								$(B)/$(JAMPG)/game/NPC_AI_Howler.o \
								$(B)/$(JAMPG)/game/NPC_AI_ImperialProbe.o \
								$(B)/$(JAMPG)/game/NPC_AI_Interrogator.o \
								$(B)/$(JAMPG)/game/NPC_AI_Jedi.o \
								$(B)/$(JAMPG)/game/NPC_AI_Mark1.o \
								$(B)/$(JAMPG)/game/NPC_AI_Mark2.o \
								$(B)/$(JAMPG)/game/NPC_AI_MineMonster.o \
								$(B)/$(JAMPG)/game/NPC_AI_Rancor.o \
								$(B)/$(JAMPG)/game/NPC_AI_Remote.o \
								$(B)/$(JAMPG)/game/NPC_AI_Seeker.o \
								$(B)/$(JAMPG)/game/NPC_AI_Sentry.o \
								$(B)/$(JAMPG)/game/NPC_AI_Sniper.o \
								$(B)/$(JAMPG)/game/NPC_AI_Stormtrooper.o \
								$(B)/$(JAMPG)/game/NPC_AI_Utils.o \
								$(B)/$(JAMPG)/game/NPC_AI_Wampa.o \
								$(B)/$(JAMPG)/game/NPC_behavior.o \
								$(B)/$(JAMPG)/game/NPC_combat.o \
								$(B)/$(JAMPG)/game/NPC_goal.o \
								$(B)/$(JAMPG)/game/NPC_misc.o \
								$(B)/$(JAMPG)/game/NPC_move.o \
								$(B)/$(JAMPG)/game/NPC_reactions.o \
								$(B)/$(JAMPG)/game/NPC_senses.o \
								$(B)/$(JAMPG)/game/NPC_sounds.o \
								$(B)/$(JAMPG)/game/NPC_spawn.o \
								$(B)/$(JAMPG)/game/NPC_stats.o \
								$(B)/$(JAMPG)/game/NPC_utils.o \
								$(B)/$(JAMPG)/game/NPC.o \
								$(B)/$(JAMPG)/game/SpeederNPC.o \
								$(B)/$(JAMPG)/game/tri_coll_test.o \
								$(B)/$(JAMPG)/game/w_force.o \
								$(B)/$(JAMPG)/game/w_saber.o \
								$(B)/$(JAMPG)/game/WalkerNPC.o \
								$(B)/$(JAMPG)/qcommon/q_math.o \
								$(B)/$(JAMPG)/qcommon/q_shared.o

OPENJKDED_NAME				= $(B)/$(INST)/openjkded.i386
OPENJKDED_CFLAGS			= -msse2 -Wall -Wno-comment -fvisibility=hidden -fsigned-char -mstackrealign -mfpmath=sse -O2 -DNDEBUG -O2 -I. -I../lib
OPENJKDED_CXXFLAGS		= -msse2 -Wall -Wno-invalid-offsetof -Wno-write-strings -Wno-comment -fvisibility=hidden -fvisibility-inlines-hidden -fsigned-char -mstackrealign -mfpmath=sse -O2 -DNDEBUG -O2 -I. -I../shared -I../lib
OPENJKDED_CXXDEFINES	= -DARCH_STRING=\"i386\" -DDEDICATED -DFINAL_BUILD -D_CONSOLE
OPENJKDED_LDFLAGS		= -m32 -ldl -lz
OPENJKDED_OBJS				= 	$(B)/$(OPENJKDED)/botlib/be_aas_bspq3.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_cluster.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_debug.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_entity.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_file.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_main.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_move.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_optimize.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_reach.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_route.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_routealt.o \
											$(B)/$(OPENJKDED)/botlib/be_aas_sample.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_char.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_chat.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_gen.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_goal.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_move.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_weap.o \
											$(B)/$(OPENJKDED)/botlib/be_ai_weight.o \
											$(B)/$(OPENJKDED)/botlib/be_ea.o \
											$(B)/$(OPENJKDED)/botlib/be_interface.o \
											$(B)/$(OPENJKDED)/botlib/l_crc.o \
											$(B)/$(OPENJKDED)/botlib/l_libvar.o \
											$(B)/$(OPENJKDED)/botlib/l_log.o \
											$(B)/$(OPENJKDED)/botlib/l_memory.o \
											$(B)/$(OPENJKDED)/botlib/l_precomp.o \
											$(B)/$(OPENJKDED)/botlib/l_script.o \
											$(B)/$(OPENJKDED)/botlib/l_struct.o \
											$(B)/$(OPENJKDED)/ghoul2/G2_gore.o \
											$(B)/$(OPENJKDED)/icarus/BlockStream.o \
											$(B)/$(OPENJKDED)/icarus/GameInterface.o \
											$(B)/$(OPENJKDED)/icarus/Instance.o \
											$(B)/$(OPENJKDED)/icarus/Interface.o \
											$(B)/$(OPENJKDED)/icarus/Memory.o \
											$(B)/$(OPENJKDED)/icarus/Q3_Interface.o \
											$(B)/$(OPENJKDED)/icarus/Q3_Registers.o \
											$(B)/$(OPENJKDED)/icarus/Sequence.o \
											$(B)/$(OPENJKDED)/icarus/Sequencer.o \
											$(B)/$(OPENJKDED)/icarus/TaskManager.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/png.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngerror.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngget.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngmem.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngpread.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngread.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngrio.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngrtran.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngrutil.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngset.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngtrans.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngwio.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngwrite.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngwtran.o \
											$(B)/$(OPENJKDED)/$(LIB)/libpng/pngwutil.o \
											$(B)/$(OPENJKDED)/null/null_client.o \
											$(B)/$(OPENJKDED)/null/null_input.o \
											$(B)/$(OPENJKDED)/null/null_renderer.o \
											$(B)/$(OPENJKDED)/null/null_snddma.o \
											$(B)/$(OPENJKDED)/qcommon/cm_load.o \
											$(B)/$(OPENJKDED)/qcommon/cm_patch.o \
											$(B)/$(OPENJKDED)/qcommon/cm_polylib.o \
											$(B)/$(OPENJKDED)/qcommon/cm_test.o \
											$(B)/$(OPENJKDED)/qcommon/cm_trace.o \
											$(B)/$(OPENJKDED)/qcommon/cmd.o \
											$(B)/$(OPENJKDED)/qcommon/common.o \
											$(B)/$(OPENJKDED)/qcommon/cvar.o \
											$(B)/$(OPENJKDED)/qcommon/files.o \
											$(B)/$(OPENJKDED)/qcommon/GenericParser2.o \
											$(B)/$(OPENJKDED)/qcommon/huffman.o \
											$(B)/$(OPENJKDED)/qcommon/matcomp.o \
											$(B)/$(OPENJKDED)/qcommon/md4.o \
											$(B)/$(OPENJKDED)/qcommon/md5.o \
											$(B)/$(OPENJKDED)/qcommon/msg.o \
											$(B)/$(OPENJKDED)/qcommon/net_chan.o \
											$(B)/$(OPENJKDED)/qcommon/net_ip.o \
											$(B)/$(OPENJKDED)/qcommon/persistence.o \
											$(B)/$(OPENJKDED)/qcommon/q_math.o \
											$(B)/$(OPENJKDED)/qcommon/q_shared.o \
											$(B)/$(OPENJKDED)/qcommon/RoffSystem.o \
											$(B)/$(OPENJKDED)/qcommon/stringed_ingame.o \
											$(B)/$(OPENJKDED)/qcommon/stringed_interface.o \
											$(B)/$(OPENJKDED)/qcommon/vm.o \
											$(B)/$(OPENJKDED)/qcommon/z_memman_pc.o \
											$(B)/$(OPENJKDED)/rd-dedicated/G2_API.o \
											$(B)/$(OPENJKDED)/rd-dedicated/G2_bolts.o \
											$(B)/$(OPENJKDED)/rd-dedicated/G2_bones.o \
											$(B)/$(OPENJKDED)/rd-dedicated/G2_misc.o \
											$(B)/$(OPENJKDED)/rd-dedicated/G2_surfaces.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_backend.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_ghoul2.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_init.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_main.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_mesh.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_model.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_shader.o \
											$(B)/$(OPENJKDED)/rd-dedicated/tr_skin.o \
											$(B)/$(OPENJKDED)/server/NPCNav/navigator.o \
											$(B)/$(OPENJKDED)/server/sv_bot.o \
											$(B)/$(OPENJKDED)/server/sv_ccmds.o \
											$(B)/$(OPENJKDED)/server/sv_client.o \
											$(B)/$(OPENJKDED)/server/sv_game.o \
											$(B)/$(OPENJKDED)/server/sv_gameapi.o \
											$(B)/$(OPENJKDED)/server/sv_init.o \
											$(B)/$(OPENJKDED)/server/sv_main.o \
											$(B)/$(OPENJKDED)/server/sv_net_chan.o \
											$(B)/$(OPENJKDED)/server/sv_snapshot.o \
											$(B)/$(OPENJKDED)/server/sv_world.o \
											$(B)/$(OPENJKDED)/shared/sys/con_log.o \
											$(B)/$(OPENJKDED)/shared/sys/con_tty.o \
											$(B)/$(OPENJKDED)/shared/sys/snapvector.o \
											$(B)/$(OPENJKDED)/shared/sys/sys_main.o \
											$(B)/$(OPENJKDED)/shared/sys/sys_unix.o \
											$(B)/$(OPENJKDED)/shared/sys/sys_event.o \
											$(B)/$(OPENJKDED)/$(LIB)/minizip/ioapi.o \
											$(B)/$(OPENJKDED)/$(LIB)/minizip/unzip.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/adler32.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/compress.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/crc32.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/deflate.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/gzclose.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/gzlib.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/gzread.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/gzwrite.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/infback.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/inffast.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/inflate.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/inftrees.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/trees.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/uncompr.o \
											$(B)/$(OPENJKDED)/$(LIB)/zlib/zutil.o 

GAME_CFLAGS += -D__linux__
OPENJKDED_CFLAGS += -D__linux__

all: makedirs jampgame openjkded

makedirs:
	@if [ ! -d $(B) ];then mkdir $(B);fi
	@if [ ! -d $(B)/$(INST) ];then mkdir $(B)/$(INST);fi
	@if [ ! -d $(B)/$(INST)/$(BASE) ];then mkdir $(B)/$(INST)/$(BASE);fi
	@if [ ! -d $(B)/$(JAMPG) ];then mkdir $(B)/$(JAMPG);fi
	@if [ ! -d $(B)/$(JAMPG)/game ];then mkdir $(B)/$(JAMPG)/game;fi
	@if [ ! -d $(B)/$(JAMPG)/qcommon ];then mkdir $(B)/$(JAMPG)/qcommon;fi
	@if [ ! -d $(B)/$(OPENJKDED) ];then mkdir $(B)/$(OPENJKDED);fi
	@if [ ! -d $(B)/$(OPENJKDED)/ghoul2 ];then mkdir $(B)/$(OPENJKDED)/ghoul2;fi
	@if [ ! -d $(B)/$(OPENJKDED)/botlib ];then mkdir $(B)/$(OPENJKDED)/botlib;fi
	@if [ ! -d $(B)/$(OPENJKDED)/icarus ];then mkdir $(B)/$(OPENJKDED)/icarus;fi
	@if [ ! -d $(B)/$(OPENJKDED)/$(LIB) ];then mkdir $(B)/$(OPENJKDED)/$(LIB);fi
	@if [ ! -d $(B)/$(OPENJKDED)/$(LIB)/libpng ];then mkdir $(B)/$(OPENJKDED)/$(LIB)/libpng;fi
	@if [ ! -d $(B)/$(OPENJKDED)/$(LIB)/minizip ];then mkdir $(B)/$(OPENJKDED)/$(LIB)/minizip;fi
	@if [ ! -d $(B)/$(OPENJKDED)/null ];then mkdir $(B)/$(OPENJKDED)/null;fi
	@if [ ! -d $(B)/$(OPENJKDED)/qcommon ];then mkdir $(B)/$(OPENJKDED)/qcommon;fi
	@if [ ! -d $(B)/$(OPENJKDED)/rd-dedicated ];then mkdir $(B)/$(OPENJKDED)/rd-dedicated;fi
	@if [ ! -d $(B)/$(OPENJKDED)/server ];then mkdir $(B)/$(OPENJKDED)/server;fi
	@if [ ! -d $(B)/$(OPENJKDED)/server/NPCNav ];then mkdir $(B)/$(OPENJKDED)/server/NPCNav;fi
	@if [ ! -d $(B)/$(OPENJKDED)/shared ];then mkdir $(B)/$(OPENJKDED)/shared;fi
	@if [ ! -d $(B)/$(OPENJKDED)/shared/sys ];then mkdir $(B)/$(OPENJKDED)/shared/sys;fi
	@if [ ! -d $(B)/$(OPENJKDED)/$(LIB)/zlib ];then mkdir $(B)/$(OPENJKDED)/$(LIB)/zlib;fi

#
# GAME RULES
#

jampgame: $(GAME_NAME)

$(GAME_NAME): $(GAME_OBJS)
	$(CC) -o $(GAME_NAME) $(GAME_OBJS) $(GAME_LDFLAGS)

$(B)/$(JAMPG)/game/%.o: game/%.c
	$(CC) $(GAME_CFLAGS) $(GAME_CDEFINES) -c $< -o $@

$(B)/$(JAMPG)/qcommon/q_%.o: qcommon/q_%.c
	$(CC) $(GAME_CFLAGS) $(GAME_CDEFINES) -c $< -o $@

#
# OPENJKDED RULES
#

openjkded: $(OPENJKDED_NAME)

$(OPENJKDED_NAME): $(OPENJKDED_OBJS)
	$(CXX) -o $(OPENJKDED_NAME) $(OPENJKDED_OBJS) $(OPENJKDED_LDFLAGS)

$(B)/$(OPENJKDED)/botlib/%.o: botlib/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -DBOTLIB -c $< -o $@

$(B)/$(OPENJKDED)/ghoul2/%.o: ghoul2/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@
	
$(B)/$(OPENJKDED)/icarus/%.o: icarus/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/$(LIB)/libpng/%.o: ../$(LIB)/libpng/%.c
	$(CC) $(OPENJKDED_CFLAGS) -c $< -o $@
	
$(B)/$(OPENJKDED)/null/%.o: null/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/qcommon/%.o: qcommon/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/rd-dedicated/%.o: rd-dedicated/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/server/%.o: server/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/server/NPCNav/%.o: server/NPCNav/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@

$(B)/$(OPENJKDED)/shared/sys/%.o: ../shared/sys/%.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@
	
$(B)/$(OPENJKDED)/sys/snapvector.o: sys/snapvector.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@
	
$(B)/$(OPENJKDED)/$(LIB)/minizip/ioapi.o: ../$(LIB)/minizip/ioapi.c
	$(CC) $(OPENJKDED_CFLAGS) -c $< -o $@
	
$(B)/$(OPENJKDED)/$(LIB)/minizip/unzip.o: ../$(LIB)/minizip/unzip.cpp
	$(CXX) $(OPENJKDED_CFLAGS) $(OPENJKDED_CXXFLAGS) $(OPENJKDED_CXXDEFINES) -c $< -o $@
	
$(B)/$(OPENJKDED)/$(LIB)/zlib/%.o: ../$(LIB)/zlib/%.c
	$(CC) $(OPENJKDED_CFLAGS) -c $< -o $@

clean:
	rm -rf $(B)

clean_jampgame:
	$(RM) $(GAME_OBJS) \
	$(GAME_NAME)

clean_openjkded:
	$(RM) $(OPENJKDED_OBJS) \
	$(OPENJKDED_NAME)
cmake_minimum_required(VERSION 3.21.0)

# Project name and version
project(app VERSION 0.0.1)

# Specify the source directory
set(SRC_DIR ${CMAKE_SOURCE_DIR}/src)

# Copy data directory to build directory for linking
# file(COPY ${CMAKE_SOURCE_DIR}/data DESTINATION ${CMAKE_BINARY_DIR})

# Add the library
# file(GLOB_RECURSE SOURCES "${SRC_DIR}/*.cpp" "${SRC_DIR}/*.h")
add_executable(headless-angband
  src/buildid.c
  src/cave-map.c
  src/cave-square.c
  src/cave-view.c
  src/cave.c
  src/cmd-cave.c
  src/cmd-core.c
  src/cmd-misc.c
  src/cmd-obj.c
  src/cmd-pickup.c
  src/cmd-spoil.c
  src/cmd-wizard.c
  src/datafile.c
  src/debug.c
  src/effect-handler-attack.c
  src/effect-handler-general.c
  src/effects.c
  src/effects-info.c
  src/game-event.c
  src/game-input.c
  src/game-world.c
  src/gen-cave.c
  src/gen-chunk.c
  src/gen-monster.c
  src/gen-room.c
  src/gen-util.c
  src/generate.c
  src/grafmode.c
  src/guid.c
  src/init.c
  src/load.c
  src/main-gcu.c
  src/main.c
  src/message.c
  src/mon-attack.c
  src/mon-blows.c
  src/mon-desc.c
  src/mon-group.c
  src/mon-init.c
  src/mon-list.c
  src/mon-lore.c
  src/mon-make.c
  src/mon-move.c
  src/mon-msg.c
  src/mon-predicate.c
  src/mon-spell.c
  src/mon-summon.c
  src/mon-timed.c
  src/mon-util.c
  src/obj-chest.c
  src/obj-curse.c
  src/obj-desc.c
  src/obj-gear.c
  src/obj-ignore.c
  src/obj-info.c
  src/obj-init.c
  src/obj-knowledge.c
  src/obj-list.c
  src/obj-make.c
  src/obj-pile.c
  src/obj-power.c
  src/obj-properties.c
  src/obj-randart.c
  src/obj-slays.c
  src/obj-tval.c
  src/obj-util.c
  src/option.c
  src/parser.c
  src/player-attack.c
  src/player-birth.c
  src/player-calcs.c
  src/player-class.c
  src/player-history.c
  src/player-path.c
  src/player-properties.c
  src/player-quest.c
  src/player-race.c
  src/player-spell.c
  src/player-timed.c
  src/player-util.c
  src/player.c
  src/project-feat.c
  src/project-mon.c
  src/project-obj.c
  src/project-player.c
  src/project.c
  src/randname.c
  src/save.c
  src/save-charoutput.c
  src/savefile.c
  src/score.c
  src/sound-core.c
  src/source.c
  src/store.c
  src/target.c
  src/trap.c
  src/ui-birth.c
  src/ui-command.c
  src/ui-context.c
  src/ui-curse.c
  src/ui-death.c
  src/ui-display.c
  src/ui-effect.c
  src/ui-entry-combiner.c
  src/ui-entry-renderers.c
  src/ui-entry.c
  src/ui-equip-cmp.c
  src/ui-event.c
  src/ui-game.c
  src/ui-help.c
  src/ui-history.c
  src/ui-init.c
  src/ui-input.c
  src/ui-keymap.c
  src/ui-knowledge.c
  src/ui-map.c
  src/ui-menu.c
  src/ui-mon-list.c
  src/ui-mon-lore.c
  src/ui-obj-list.c
  src/ui-object.c
  src/ui-options.c
  src/ui-output.c
  src/ui-player-properties.c
  src/ui-player.c
  src/ui-prefs.c
  src/ui-score.c
  src/ui-signals.c
  src/ui-spell.c
  src/ui-spoil.c
  src/ui-store.c
  src/ui-target.c
  src/ui-term.c
  src/ui-visuals.c
  src/ui-wizard.c
  src/wiz-debug.c
  src/wiz-spoil.c
  src/wiz-stats.c
  src/z-bitflag.c
  src/z-color.c
  src/z-dice.c
  src/z-expression.c
  src/z-file.c
  src/z-form.c
  src/z-quark.c
  src/z-queue.c
  src/z-rand.c
  src/z-textblock.c
  src/z-type.c
  src/z-util.c
  src/z-virt.c)

# Set include directories
target_include_directories(headless-angband PRIVATE ${SRC_DIR})
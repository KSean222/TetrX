object_dir = ../obj/
all_debug_targets = bot_types_debug.o tree_debug.o move_queue_debug.o node_queue_debug.o bot_debug.o
all_targets = bot_types.o tree.o move_queue.o node_queue.o bot.o

all_debug:
	make $(all_debug_targets)

%_debug.o: %.c
	gcc $(debug_flags) -c $< -o $(object_dir)$@

all:
	make $(all_targets)

%.o: %.c
	gcc $(normal_flags) -c $< -o $(object_dir)$@

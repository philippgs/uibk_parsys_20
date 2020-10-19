CC=gcc
CC_FLAGS=-O2 -std=c99 -Wall -Wextra -pedantic

.PHONEY: all
all: heat_stencil_1D_seq

heat_stencil_1D_seq: heat_stencil_1D_seq.c
	@$(CC) $(CC_FLAGS) $< -o heat_stencil_1D_seq

.PHONEY: clean
clean:
	@rm heat_stencil_1D_seq

.PHONEY: run
run: all
	@echo "Sequential:"
	@./heat_stencil_1D_seq
	@echo

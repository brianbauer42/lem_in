# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: bbauer <marvin@42.fr>                      +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2016/11/03 16:20:35 by bbauer            #+#    #+#              #
#    Updated: 2017/05/26 15:21:07 by bbauer           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a
SRC = ft_atoi.c ft_bzero.c ft_isalnum.c ft_isalpha.c ft_isascii.c ft_isdigit.c \
	  ft_ishex.c ft_isprint.c ft_itoa.c ft_itoa_base.c ft_itoa_base_intmax.c \
	  ft_itoa_base_uintmax.c ft_itoa_base_ull.c ft_lst_append.c \
	  ft_lst_free_contents.c ft_lst_len.c ft_lstadd.c ft_lstdel.c \
	  ft_lstdelone.c ft_lstiter.c ft_lstmap.c ft_lstnew.c ft_memalloc.c \
	  ft_memccpy.c ft_memchr.c ft_memcmp.c ft_memcpy.c ft_memdel.c \
	  ft_memmove.c ft_memset.c ft_nbrlen.c ft_putchar.c ft_putchar_fd.c \
	  ft_putendl.c ft_putendl_fd.c ft_putnbr.c ft_putnbr_fd.c ft_putstr.c \
	  ft_putstr_fd.c ft_realloc.c ft_strcat.c ft_strchr.c ft_strclr.c \
	  ft_strcmp.c ft_strcpy.c ft_strdel.c ft_strdup.c ft_strequ.c ft_striter.c \
	  ft_striteri.c ft_strjoin.c ft_strlcat.c ft_strlen.c ft_strmap.c \
	  ft_strmapi.c ft_strncat.c ft_strncmp.c ft_strncpy.c ft_strndup.c \
	  ft_strnequ.c ft_strnew.c ft_strnstr.c ft_strrchr.c ft_strsplit.c \
	  ft_strstr.c ft_strsub.c ft_strtrim.c ft_tolower.c ft_tolower_str.c \
	  ft_toupper.c ft_toupper_str.c ft_utf8charencode.c ft_utf8charsize.c \
	  ft_utf8strencode.c ft_utf8strnencode.c ft_wchar_memset.c ft_wcharbits.c \
	  ft_wcharsize_utf8.c ft_wctomb.c ft_wrdcnt.c ft_wrdcntd.c ft_wrdlen.c \
	  ft_wrdsplit.c ft_wstrcpy.c ft_wstrdup.c ft_wstrlen.c ft_wstrndup.c \
	  ft_wstrnsize_utf8.c ft_wstrsize_utf8.c get_next_line.c ft_strtok.c \
	  ft_strcdup.c ft_tab_add_one.c ft_tab_cat.c ft_tab_del.c ft_tab_dup.c \
	  ft_tab_ncat.c ft_tab_new.c ft_tab_rem_one.c ft_print_tab.c ft_strcspn.c \
	  ft_strbeginequ.c ft_smallest_int.c ft_tab_len.c ft_ints_are_sorted.c \
	  ft_print_arr.c ft_ints_are_rev_sorted.c ft_int_sort.c ft_int_sort_rev.c \
	  ft_atol.c ft_char_count.c

OBJDIR = ./obj/
OPT = $(SRC:.c=.o)
HEADER = ./libft.h
FLAGS = -c -Wall -Wextra -Werror

all: $(NAME)

$(NAME):
	@echo "Compiling libft"
	@gcc $(OPTIONS) $(SRC) $(FLAGS)
	@ar rc $(NAME) $(OPT)
	@mkdir $(OBJDIR)
	@mv $(OPT) $(OBJDIR)
	@ranlib $(NAME)
	@echo "lift: SUCCESS!"

clean:
	@echo "Cleaning libft"
	@/bin/rm -rf $(OBJDIR)

fclean: clean
	@echo "FCleaning libft"
	@/bin/rm -f $(NAME)
	@/bin/rm -f libft.h.gch

re: fclean all

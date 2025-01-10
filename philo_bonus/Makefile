NAME = philo_bonus
OBJ = $(SRC:.c=.o)

SRC = philo_bonus.c utils_bonus.c setup_bonus.c routine_bonus.c

CC = cc
CFLAGS = -Wall -Werror -Wextra

COMP = $(CC) $(CFLAGS)

RM = rm -f

all:	$(NAME)

$(NAME):	$(OBJ)
		$(COMP) $(OBJ) -o $(NAME)

bonus:	$(NAME)

clean:
		$(RM) $(OBJ)
		
fclean:	clean
		$(RM) $(NAME)

re:		fclean all
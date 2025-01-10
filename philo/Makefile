NAME = philo
OBJ = $(SRC:.c=.o)

SRC = philo.c utils.c setup.c routine.c

CC = cc
CFLAGS = -Wall -Werror -Wextra

COMP = $(CC) $(CFLAGS)

RM = rm -f

all:	$(NAME)

$(NAME):	$(OBJ)
		$(COMP) $(OBJ) -o $(NAME)

clean:
		$(RM) $(OBJ)
		
fclean:	clean
		$(RM) $(NAME)

re:		fclean all
# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: slammari <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/01/18 23:19:23 by slammari          #+#    #+#              #
#    Updated: 2022/01/20 15:19:39 by slammari         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #


INC = minitalk.h
INC_BONUS = minitalk_bonus.h

CFLAGS = -Wall -Wextra -Werror


all : server client

bonus: server_bonus client_bonus

server: server.c minitalk_utils.c $(INC)
	cc $(CFLAGS) server.c minitalk_utils.c -o server

client: client.c minitalk_utils.c $(INC)
	cc $(CFLAGS) client.c minitalk_utils.c -o client
	
server_bonus: server_bonus.c minitalk_utils.c $(INC_BONUS)
	cc $(CFLAGS) server_bonus.c minitalk_utils.c -o server_bonus

client_bonus: client_bonus.c minitalk_utils.c $(INC_BONUS)
	cc $(CFLAGS)  client_bonus.c minitalk_utils.c -o client_bonus

clean:
	
fclean : clean
	rm -rf server server_bonus client client_bonus

re : fclean all

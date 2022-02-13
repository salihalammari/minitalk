# minitalk

Execution

makeor make allormake bonus

bash ./server

bash ./client [SERVER PID] [SEND MESSAGE]

assignment requirements

When the client is running, it must display the PID.

. The server MUST display the string when it is received.

. For communication between server and client, only SIGUSR1 and SIGUSR2 signals among UNIX signals can be used.

. The server must be able to display the string at a very high speed.

. I need to be able to display a string of 100 characters in 1 second.

. The server should be able to receive strings consecutively from multiple clients without the need for a restart.

  Bonus

Addition of small acknowledgment system (acknowledgment between server/client

) Apply half-duplex communication method instead of simplex communication.

Try to support Unicode characters as well.

🖤∑∞☞★⚝✅🔥⌚☣☮🌏📱Ⅻ🚀€🍔🍦👑⚽🎵🎧♻

sigaction
SA_SIGINFO
If the SA_SIGINFO flag is specified in sa_flags, the cause of the signal can be known.
When designating a signal handler in the sigaction structure, use sa_sigaction instead of sa_handler.
A signal handler is defined in a form that receives three arguments as follows.

      void handler(int signo, siginfo_t *siginfo, ucontext_t *context);
      
sigaction:

. SA_SIGINFO

If the SA_SIGINFO flag is specified in sa_flags, the cause of the signal can be known.
When designating a signal handler in the sigaction structure, use sa_sigaction instead of sa_handler.
A signal handler is defined in a form that receives three arguments as follows.

      void handler(int signo, siginfo_t *siginfo, ucontext_t *context);


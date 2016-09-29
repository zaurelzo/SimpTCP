# SimpTCP
During my third year at INSA Toulouse, we had to design a network protocol which mixed TC and UDP features. This network protocol works with SYN, SYN-ACK, ACK when establishing the connexion between a custom and a server. The custom can send PDU package and the server received this package and send an ACK.  
We implemented the following functions in the file src/simptcp_lib.c :
closed_simptcp_socket_state_active_open, 
closed_simptcp_socket_state_passive_open, 
listen_simptcp_socket_state_accept, 
listen_simptcp_socket_state_close, 
listen_simptcp_socket_state_process_simptcp_pdu, 
synsent_simptcp_socket_state_process_simptcp_pdu, 
synsent_simptcp_socket_state_handle_timeout, 
synrcvd_simptcp_socket_state_process_simptcp_pdu, 
synrcvd_simptcp_socket_state_handle_timeout, 
established_simptcp_socket_state_send, 
established_simptcp_socket_state_recv, 
established_simptcp_socket_state_shutdown, 
established_simptcp_socket_state_process_simptcp_pdu, 
established_simptcp_socket_state_handle_timeout, 
finwait1_simptcp_socket_state_process_simptcp_pdu, 
timewait_simptcp_socket_state_process_simptcp_pdu, 
timewait_simptcp_socket_state_handle_timeout.

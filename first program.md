## 1. Write a ALP to print your name

''' assembly

    section .data
    msg db 'avishkar kumbhar'
    msg_len equ $-msg

section .text
    global _start
_start:
    mov rax, 1
    mov rdi, 1
    mov rsi, msg
    mov rdx, msg_len
    syscall


    mov rax, 60
    mov rdi, 0
    syscall
    
'''
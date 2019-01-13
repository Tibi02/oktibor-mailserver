# oktibor-mailserver
Poste.io docker

## Usage

#### Get latest image
```
docker pull analogic/poste.io
```

#### Start container
```
docker-compose up -d
```

## Ports
Ports which are opened by poste.io

Port | Purpose
--- | --- 
25 | SMTP - mostly processing incoming mails
110 | POP3 - standard protocol for accessing mailbox, STARTTLS is required before client auth
143 | IMAP - standard protocol for accessing mailbox, STARTTLS is required before client auth
465 | SMTPS - Legacy SMTPs port
587 | MSA - SMTP port used primarily for email clients after STARTTLS and auth
993 | IMAPS - alternative port for IMAP encrypted since connection
995 | POP3S - encrypted POP3 since connections
4190 | Sieve - remote sieve settings

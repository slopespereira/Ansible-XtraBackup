# XtraBackup Com Ansible
Projeto desenvolvido para automatizar os backups do MySQL com XtraBackup, os backups serão padronizados independendte da versão do MySQL, caso o XtraBackup não esteija instalado, ele será instalado automaticamente.
### Features
- Verifica versão do Sistema Operacional
- Checa a versão do MySQL
- Checa se o  MySQL está UP
- Configura repositório do XtraBackup
- Instala o XtraBackup conforma versão do MySQL
- Executa o backup conforme versão do MySQL
- Valida o backup, em caso de falha finaliza a playbook



###Reference

[Percona XtraBackup 2.4 Documentation](https://www.percona.com/doc/percona-xtrabackup/2.4/backup_scenarios/full_backup.html#restoring-a-backup "Percona XtraBackup 2.4 Documentation")

[Percona XtraBackup 8.0 Documentation](https://www.percona.com/doc/percona-xtrabackup/8.0/index.html "Percona XtraBackup 8.0 Documentation")



###Executar a Playbook


`$ ansible-playbook -i hosts site.yml -u USER -l xtrabackup -k`

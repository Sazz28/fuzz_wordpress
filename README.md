# fuzz_wordpress
WordPress Sensitive Path Scanner 🔍 A comprehensive wordlist and scanning tool for identifying sensitive and misconfigured paths in WordPress installations

WordPress Sensitive Path Scanner 🔍 A comprehensive wordlist and scanning tool for identifying sensitive and misconfigured paths in WordPress installations
his repository provides a curated wordlist of high-risk and often-misconfigured WordPress file paths that could expose critical configuration files, credentials, logs, backups, and source code artifacts if left accessible. Combined with tools like gobuster, ffuf, or dirsearch, it helps penetration testers, bug bounty hunters, and sysadmins perform focused enumeration of:

wp-config.php, .env, and other config leaks
Misplaced database dumps (.sql, .gz, .zip)
Debug logs and error logs
Backup directories in uploads or custom plugin paths
Exposed .git/, CI/CD pipelines, and test artifacts

Includes:
wordpress-sensitive-paths.txt – 200+ curated paths
gobuster-ready-wordlist.txt – Format optimized for web fuzzing
Sample usage scripts for gobuster, ffuf, and curl
Nginx & Apache hardening snippets to block common leak points

Use Cases:
Offensive Security Recon
Bug Bounty Path Enumeration
WordPress Hardening Audits

Note: Use only with explicit authorization. This tool is designed for ethical security testing and awareness.

Configuration @ Secrets 
/wp-config.php	

/.env	

/wp-config-sample.php	

/config/database.yml, /config.php	.

/local-config.php, /config-local.php	


/wp-content/debug.log	

/error_log, /php_errorlog, /logs/error.log	

/wp-content/*.log, /wp-content/uploads/*.log	

/backup/, /backups/, /wp-content/backups/	

/wp-content/uploads/backups/	

/*.zip, /*.tar.gz, /*.sql, /*.bak	.

/wp-backup.zip, /db-backup.sql	

/.git/, /.svn/, /.hg/	

/.git/config, /.git/logs/HEAD, /.git/index	

/composer.json, /composer.lock	.

/package.json, /webpack.config.js	

/node_modules/	




/readme.html, /license.txt, /changelog.txt

/phpinfo.php, /info.php	

/test.php, /test.php~, /1.php, /phpinfo()	

/old/, /dev/, /staging/	  

/wp-admin/install.php	

/wp-admin/upgrade.php	

/wp-admin/setup-config.php	

/wp-admin/includes/upgrade.php	

/wp-content/plugins/**/debug.log	

/wp-content/plugins/**/config.php	

/wp-content/themes/**/log/	

/wp-content/plugins/**/.env	

/phpunit.xml, /phpunit.xml.dist	

/tests/, /spec/, /__tests__/	

/ci/, /jenkins/, .travis.yml, .gitlab-ci.yml	

.dockerignore, docker-compose.yml	


# RegX

RegX is a collection of Regex strings gathered from various publicly available sources that can be used for pentesting, source code review, and bug hunting.

| Product | Regex String |
| - | - |
| AWS API Key | ```AKIA[0-9A-Z]{16}``` |
| AWS ARN | ```arn:aws:organizations::\d{12}:account\/o-[a-z0-9]{10,32}\/\d{12}``` |
| AWS Access Key ID | ```(?<![A-Z0-9])[A-Z0-9]{20}(?![A-Z0-9])``` |
| AWS CLI Credentials File | ```\.?aws/credentials``` |
| AWS Secret Access Key | ```(?<![A-Za-z0-9/+=])[A-Za-z0-9/+=]{40}(?![A-Za-z0-9/+=])``` |
| AWS Session Token | ```(?<![A-Za-z0-9/+=])[A-Za-z0-9/+=]{16,}(?<![A-Za-z0-9/+=])``` |
| Amazon AWS Access Key ID | ``` ([^A-Z0-9]\|^)(AKIA\|A3T\|AGPA\|AIDA\|AROA\|AIPA\|ANPA\|ANVA\|ASIA)[A-Z0-9]{12,} ``` |
| Amazon AWS S3 Bucket | ```//s3-[a-z0-9-]+\\.amazonaws\\.com/[a-z0-9._-]+``` |
| Amazon AWS S3 Bucket | ```//s3\\.amazonaws\\.com/[a-z0-9._-]+``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3-[a-z0-9-]\\.amazonaws\\.com``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3-website[.-](eu\|ap\|us\|ca\|sa\|cn)``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3\\.amazonaws\\.com``` |
| Amazon MWS Auth Token | ```amzn\.mws\.[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}``` |
| Apache htpasswd File | ```\.?htpasswd``` |
| Artifactory API Token | ```(?:\\s\|=\|:\|\"\|^)AKC[a-zA-Z0-9]{10,}``` |
| Artifactory Password | ```(?:\\s\|=\|:\|\"\|^)AP[\\dABCDEF][a-zA-Z0-9]{8,}``` |
| Authorization Basic | ```basic\\s[a-zA-Z0-9_\\-:\\.=]+``` |
| Authorization Bearer | ```Bearer\s[A-Za-z0-9\-_=]+\.[A-Za-z0-9\-_=]+(\.[A-Za-z0-9\-_.+/=]+)?``` |
| Authorization Bearer | ```Bearer\s[\d\|a-f]{8}-([\d\|a-f]{4}-){3}[\d\|a-f]{12}``` |
| Authorization Bearer | ```bearer\\s[a-zA-Z0-9_\\-:\\.=]+``` |
| Authorization Splunk | ```Splunk\s(\{){0,1}[0-9a-fA-F]{8}\-[0-9a-fA-F]{4}\-[0-9a-fA-F]{4}\-[0-9a-fA-F]{4}\-[0-9a-fA-F]{12}(\}){0,1}``` |
| Basic Auth Credentials | ```(?<=:\/\/)[a-zA-Z0-9]+:[a-zA-Z0-9]+@[a-zA-Z0-9]+\\.[a-zA-Z]+``` |
| Chef Private Key | ```\.?chef/(.*)\.pem``` |
| Cloudinary Basic Auth | ```cloudinary:\/\/[0-9]{15}:[0-9A-Za-z]+@[a-z]+``` |
| Configuration File for auto-login Process | ```(\.\|_)?netrc``` |
| DBeaver SQL Database Manager Configuration File | ```\.?dbeaver-data-sources(-[0-9]+)?\.xml``` |
| DigitalOcean doctl command-line Client Configuration File | ```doctl/config\.yaml``` |
| Discord BOT Token | ```((?:N\|M\|O)[a-zA-Z0-9]{23}\\.[a-zA-Z0-9-_]{6}\\.[a-zA-Z0-9-_]{27})$``` |
| Docker Configuration File | ```\.?dockercfg``` |
| Environment Configuration File | ```\.env``` |
| Facebook Access Token | ```EAACEdEose0cBA[0-9A-Za-z]+``` |
| Facebook ClientID | ```[f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K](.{0,20})?['\"][0-9]{13,17}``` |
| Facebook OAuth | ```[f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K].*['\|\"][0-9a-f]{32}['\|\"]``` |
| Facebook Secret Key | ```([f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K]\|[f\|F][b\|B])(.{0,20})?['\"][0-9a-f]{32}``` |
| Firebase | ```[a-z0-9.-]+\\.firebaseio\\.com``` |
| GNOME Keyring Database File | ```key(store\|ring)[\W]+``` |
| Generic API Key | ```[a\|A][p\|P][i\|I][_]?[k\|K][e\|E][y\|Y].*['\|\"][0-9a-zA-Z]{32,45}['\|\"]``` |
| Generic Secret | ```[s\|S][e\|E][c\|C][r\|R][e\|E][t\|T].*['\|\"][0-9a-zA-Z]{32,45}['\|\"]``` |
| Git configuration File | ```\.?gitconfig``` |
| GitHub Access Token | ```([a-zA-Z0-9_-]*:[a-zA-Z0-9_-]+@github.com*)$``` |
| GitHub | ```[g\|G][i\|I][t\|T][h\|H][u\|U][b\|B].*['\|\"][0-9a-zA-Z]{35,40}['\|\"]``` |
| Google Cloud API Key | ```AIza[0-9A-Za-z\\-_]{35}``` |
| Google Cloud Platform OAuth | ```[0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com``` |
| Google Cloud Platform Service Account | ```\"type\": \"service_account\"``` |
| Google OAuth Access Token | ```ya29\\.[0-9A-Za-z\\-_]+``` |
| Google OAuth Key | ```[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com``` |
| Heroku API Key | ```[h\|H][e\|E][r\|R][o\|O][k\|K][u\|U].*[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}``` |
| Heroku Key | ```(?i)heroku(.{0,20})?[''"][0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}[''"]``` |
| Hexchat/XChat IRC client server list configuration file | ```\.?xchat2?/servlist.conf``` |
| IP Address | ```(([0-9]\|[1-9][0-9]\|1[0-9]{2}\|2[0-4][0-9]\|25[0-5])\\.){3}([0-9]\|[1-9][0-9]\|1[0-9]{2}\|2[0-4][0-9]\|25[0-5])``` |
| Irssi IRC Client Configuration File | ```\.?irssi/config``` |
| JSON Web Token | ```(?i)^((?=.*[a-z])(?=.*[0-9])(?:[a-z0-9_=]+\\.){2}(?:[a-z0-9_\\-\\+\/=]*))$``` |
| KeePass Password Manager Database File | ```\.kdbx?``` |
| LinkFinder | ```(?:\"\|')(((?:[a-zA-Z]{1,10}:\/\/\|\/\/)[^\"'\/]{1,}\\.[a-zA-Z]{2,}[^\"']{0,})\|((?:\/\|\\.\\.\/\|\\.\/)[^\"'><,;\| *()(%%$^\/\\\\\\[\\]][^\"'><,;\|()]{1,})\|([a-zA-Z0-9_\\-\/]{1,}\/[a-zA-Z0-9_\\-\/]{1,}\\.(?:[a-zA-Z]{1,4}\|action)(?:[\\?\|#][^\"\|']{0,}\|))\|([a-zA-Z0-9_\\-\/]{1,}\/[a-zA-Z0-9_\\-\/]{3,}(?:[\\?\|#][^\"\|']{0,}\|))\|([a-zA-Z0-9_\\-]{1,}\\.(?:php\|asp\|aspx\|jsp\|json\|action\|html\|js\|txt\|xml)(?:[\\?\|#][^\"\|']{0,}\|)))(?:\"\|')``` |
| LinkedIn Secret Key | ```(?i)linkedin(.{0,20})?[''"][0-9a-z]{16}[''"]``` |
| Linkedin Client ID | ```(?i)linkedin(.{0,20})?(?-i)[''"][0-9a-z]{12}[''"]``` |
| Mac Address | ```(([0-9A-Fa-f]{2}[:]){5}[0-9A-Fa-f]{2}\|([0-9A-Fa-f]{2}[-]){5}[0-9A-Fa-f]{2}\|([0-9A-Fa-f]{4}[\\.]){2}[0-9A-Fa-f]{4})$``` |
| MailChimp API Key | ```[0-9a-f]{32}-us[0-9]{1,2}``` |
| Mailgun API Key | ```key-[0-9a-zA-Z]{32}``` |
| Mailto | ```(?<=mailto:)[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\.[a-zA-Z0-9.-]+``` |
| Mutt e-mail Client Configuration File | ```\.?muttrc``` |
| MySQL Client Command History File | ```(\.)?mysql_history``` |
| NPM Configuration File | ```\.?npmrc``` |
| NuGet API Key | ```oy2[a-z0-9]{43}``` |
| PGP Private Key Block | ```-----BEGIN PGP PRIVATE KEY BLOCK-----``` |
| PHP Configuration File | ```config(\.inc)?\.php``` |
| Password in URL | ```[a-zA-Z]{3,10}://[^/\\s:@]{3,20}:[^/\\s:@]{3,20}@.{1,100}[\"'\\s]``` |
| PayPal/Braintree Access Token | ```access_token\$production\$[0-9a-z]{16}\$[0-9a-f]{32}``` |
| Picatic API Key | ```sk_live_[0-9a-z]{32}``` |
| Picatic API Key | ```sk_(live\|test)_[0-9a-z]{32}``` |
| Pidgin Chat Client Account Configuration File | ```\.?purple/accounts\.xml``` |
| PostgreSQL client command History File | ```(\.)?psql_history``` |
| PostgreSQL Password File | ```(\.)?pgpass``` |
| Potential Cryptographic Private Key | ```^key(pair)?$``` |
| Private SSH key | ```^.*_dsa``` |
| Private SSH key | ```^.*_ecdsa``` |
| Private SSH key | ```^.*_ed25519``` |
| Private SSH key | ```^.*_rsa``` |
| RSA Private Key | ```-----BEGIN RSA PRIVATE KEY-----``` |
| Ruby IRB Console History File | ```(\.)?irb_history```|
| Rubygems Credentials File | ```\.?gem/credentials``` |
| S3cmd Configuration File | ```\.?s3cfg``` |
| SFTP Connection Configuration File | ```sftp-config(\.json)?``` |
| SQL Dump File | ```\.sql(dump)?``` |
| SSH DSA Private Key | ```-----BEGIN DSA PRIVATE KEY-----``` |
| SSH EC Private Key | ```-----BEGIN EC PRIVATE KEY-----``` |
| SSH Configuration File | ```\.?ssh/config$``` |
| Sauce Token | ```(?i)sauce.{0,50}("\|'\|`)?[0-9a-f-]{36}("\|'\|`)?``` |
| SendGrid API Key | ```SG\.[0-9A-Za-z\-_]{22}\.[0-9A-Za-z\-_]{43}``` |
| Shell Command Alias Configuration File | ```\.?(bash_\|zsh_)+aliases``` |
| Shell Command History File | ```\.?(bash_\|zsh_\|sh_\|z)+history``` |
| Shell Configuration File | ```\.?(bash\|zsh\|csh)rc``` |
| Shell profile configuration file | ```\.?(bash_\|zsh_)+profile``` |
| Slack Token | ```(xox[p\|b\|o\|a]-[0-9]{12}-[0-9]{12}-[0-9]{12}-[a-z0-9]{32})``` |
| Slack Token | ```(xox[pboa]-[0-9]{12}-[0-9]{12}-[0-9]{12}-[a-z0-9]{32})``` |
| Slack Webhook | ```https://hooks.slack.com/services/T[a-zA-Z0-9_]{8}/B[a-zA-Z0-9_]{8}/[a-zA-Z0-9_]{24}``` |
| SonarQube Docs API Key | ```(?i)sonar.{0,50}("\|'\|`)?[0-9a-f]{40}("\|'\|`)?```|
| Square Access Token | ```sq0atp-[0-9A-Za-z\-_]{22}``` |
| Square Access Token | ```sq0atp-[0-9A-Za-z\\-_]{22}``` |
| Square OAuth Secret | ```sq0csp-[0-9A-Za-z\-_]{43}``` |
| Square OAuth Secret | ```sq0csp-[0-9A-Za-z\\-_]{43}``` |
| StackHawk API Key | ```hawk\.[0-9A-Za-z\-_]{20}\.[0-9A-Za-z\-_]{20}``` |
| Stripe API Key | ```(?:r\|s)k_[live\|test]_[0-9a-zA-Z]{24}``` |
| Stripe API Key | ```sk_live_[0-9a-zA-Z]{24}``` |
| Stripe Restricted API Key | ```rk_live_[0-9a-zA-Z]{24}``` |
| Tugboat DigitalOcean management tool configuration | ```\.?tugboat``` |
| Twilio API Key | ```SK[0-9a-fA-F]{32}``` |
| Twitter Access Token | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R].*[1-9][0-9]+-[0-9a-zA-Z]{40}``` |
| Twitter ClientID | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R](.{0,20})?['\"][0-9a-z]{18,25}``` |
| Twitter OAuth | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R].*['\|\"][0-9a-zA-Z]{35,44}['\|\"]``` |
| Twitter Secret Key | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R](.{0,20})?['\"][0-9a-z]{35,44}``` |
| Twitter client configuration file | ```/\.?trc[\W]+``` |
| git-credential-store helper credentials file | ```\.?git-credentials``` |

# RegX

A collection of Regex strings that I use during testing.

| Product | Regex String |
| - | - |
| Amazon AWS Access Key ID | ``` ([^A-Z0-9]\|^)(AKIA\|A3T\|AGPA\|AIDA\|AROA\|AIPA\|ANPA\|ANVA\|ASIA)[A-Z0-9]{12,} ``` |
| Amazon AWS S3 Bucket | ```//s3-[a-z0-9-]+\\.amazonaws\\.com/[a-z0-9._-]+``` |
| Amazon AWS S3 Bucket | ```//s3\\.amazonaws\\.com/[a-z0-9._-]+``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3-[a-z0-9-]\\.amazonaws\\.com``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3-website[.-](eu\|ap\|us\|ca\|sa\|cn)``` |
| Amazon AWS S3 Bucket | ```[a-z0-9.-]+\\.s3\\.amazonaws\\.com``` |
| Artifactory API Token | ```(?:\\s\|=\|:\|\"\|^)AKC[a-zA-Z0-9]{10,}``` |
| Artifactory Password | ```(?:\\s\|=\|:\|\"\|^)AP[\\dABCDEF][a-zA-Z0-9]{8,}``` |
| Authorization Basic | ```basic\\s[a-zA-Z0-9_\\-:\\.=]+``` |
| Authorization Bearer | ```bearer\\s[a-zA-Z0-9_\\-:\\.=]+``` |
| AWS API Key | ```AKIA[0-9A-Z]{16}``` |
| Basic Auth Credentials | ```(?<=:\/\/)[a-zA-Z0-9]+:[a-zA-Z0-9]+@[a-zA-Z0-9]+\\.[a-zA-Z]+``` |
| Cloudinary Basic Auth | ```cloudinary:\/\/[0-9]{15}:[0-9A-Za-z]+@[a-z]+``` |
| Discord BOT Token | ```((?:N\|M\|O)[a-zA-Z0-9]{23}\\.[a-zA-Z0-9-_]{6}\\.[a-zA-Z0-9-_]{27})$``` |
| Facebook Access Token | ```EAACEdEose0cBA[0-9A-Za-z]+``` |
| Facebook ClientID | ```[f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K](.{0,20})?['\"][0-9]{13,17}``` |
| Facebook OAuth | ```[f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K].*['\|\"][0-9a-f]{32}['\|\"]``` |
| Facebook Secret Key | ```([f\|F][a\|A][c\|C][e\|E][b\|B][o\|O][o\|O][k\|K]\|[f\|F][b\|B])(.{0,20})?['\"][0-9a-f]{32}``` |
| Firebase | ```[a-z0-9.-]+\\.firebaseio\\.com``` |
| Generic API Key | ```[a\|A][p\|P][i\|I][_]?[k\|K][e\|E][y\|Y].*['\|\"][0-9a-zA-Z]{32,45}['\|\"]``` |
| Generic Secret | ```[s\|S][e\|E][c\|C][r\|R][e\|E][t\|T].*['\|\"][0-9a-zA-Z]{32,45}['\|\"]``` |
| GitHub | ```[g\|G][i\|I][t\|T][h\|H][u\|U][b\|B].*['\|\"][0-9a-zA-Z]{35,40}['\|\"]``` |
| GitHub Access Token | ```([a-zA-Z0-9_-]*:[a-zA-Z0-9_-]+@github.com*)$``` |
| Google API Key | ```AIza[0-9A-Za-z\\-_]{35}``` |
| Google Cloud Platform OAuth | ```[0-9]+-[0-9A-Za-z_]{32}\\.apps\\.googleusercontent\\.com``` |
| Google Cloud Platform Service Account | ```\"type\": \"service_account\"``` |
| Google OAuth Access Token | ```ya29\\.[0-9A-Za-z\\-_]+``` |
| Heroku API Key | ```[h\|H][e\|E][r\|R][o\|O][k\|K][u\|U].*[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}``` |
| IP Address | ```(([0-9]\|[1-9][0-9]\|1[0-9]{2}\|2[0-4][0-9]\|25[0-5])\\.){3}([0-9]\|[1-9][0-9]\|1[0-9]{2}\|2[0-4][0-9]\|25[0-5])``` |
| JSON Web Token | ```(?i)^((?=.*[a-z])(?=.*[0-9])(?:[a-z0-9_=]+\\.){2}(?:[a-z0-9_\\-\\+\/=]*))$``` |
| LinkFinder | ```(?:\"\|')(((?:[a-zA-Z]{1,10}:\/\/\|\/\/)[^\"'\/]{1,}\\.[a-zA-Z]{2,}[^\"']{0,})\|((?:\/\|\\.\\.\/\|\\.\/)[^\"'><,;\| *()(%%$^\/\\\\\\[\\]][^\"'><,;\|()]{1,})\|([a-zA-Z0-9_\\-\/]{1,}\/[a-zA-Z0-9_\\-\/]{1,}\\.(?:[a-zA-Z]{1,4}\|action)(?:[\\?\|#][^\"\|']{0,}\|))\|([a-zA-Z0-9_\\-\/]{1,}\/[a-zA-Z0-9_\\-\/]{3,}(?:[\\?\|#][^\"\|']{0,}\|))\|([a-zA-Z0-9_\\-]{1,}\\.(?:php\|asp\|aspx\|jsp\|json\|action\|html\|js\|txt\|xml)(?:[\\?\|#][^\"\|']{0,}\|)))(?:\"\|')``` |
| Mac Address | ```(([0-9A-Fa-f]{2}[:]){5}[0-9A-Fa-f]{2}\|([0-9A-Fa-f]{2}[-]){5}[0-9A-Fa-f]{2}\|([0-9A-Fa-f]{4}[\\.]){2}[0-9A-Fa-f]{4})$``` |
| MailChimp API Key | ```[0-9a-f]{32}-us[0-9]{1,2}``` |
| Mailgun API Key | ```key-[0-9a-zA-Z]{32}``` |
| Mailto | ```(?<=mailto:)[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\.[a-zA-Z0-9.-]+``` |
| Password in URL | ```[a-zA-Z]{3,10}://[^/\\s:@]{3,20}:[^/\\s:@]{3,20}@.{1,100}[\"'\\s]``` |
| PayPal Braintree Access Token | ```access_token\\$production\\$[0-9a-z]{16}\\$[0-9a-f]{32}``` |
| PGP Private Key Block | ```-----BEGIN PGP PRIVATE KEY BLOCK-----``` |
| Picatic API Key | ```sk_live_[0-9a-z]{32}``` |
| RSA Private Key | ```-----BEGIN RSA PRIVATE KEY-----``` |
| Slack Token | ```(xox[p\|b\|o\|a]-[0-9]{12}-[0-9]{12}-[0-9]{12}-[a-z0-9]{32})``` |
| Slack Webhook | ```https://hooks.slack.com/services/T[a-zA-Z0-9_]{8}/B[a-zA-Z0-9_]{8}/[a-zA-Z0-9_]{24}``` |
| Square Access Token | ```sq0atp-[0-9A-Za-z\\-_]{22}``` |
| Square OAuth Secret | ```sq0csp-[0-9A-Za-z\\-_]{43}``` |
| SSH DSA Private_Key | ```-----BEGIN DSA PRIVATE KEY-----``` |
| SSH EC Private Key | ```-----BEGIN EC PRIVATE KEY-----``` |
| Stripe API Key | ```(?:r\|s)k_[live\|test]_[0-9a-zA-Z]{24}``` |
| Stripe API Key | ```sk_live_[0-9a-zA-Z]{24}``` |
| Stripe Restricted API Key | ```rk_live_[0-9a-zA-Z]{24}``` |
| Twilio API Key | ```SK[0-9a-fA-F]{32}``` |
| Twitter Access Token | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R].*[1-9][0-9]+-[0-9a-zA-Z]{40}``` |
| Twitter ClientID | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R](.{0,20})?['\"][0-9a-z]{18,25}``` |
| Twitter OAuth | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R].*['\|\"][0-9a-zA-Z]{35,44}['\|\"]``` |
| Twitter Secret Key | ```[t\|T][w\|W][i\|I][t\|T][t\|T][e\|E][r\|R](.{0,20})?['\"][0-9a-z]{35,44}``` |
| Private SSH key | ```^.*_rsa``` |
| Private SSH key | ```^.*_dsa``` |
| Private SSH key | ```^.*_ed25519``` |
| Private SSH key | ```^.*_ecdsa``` |
| SSH configuration file | ```\.?ssh/config$``` |
| Potential Cryptographic Private Key | ```^key(pair)?$``` |
| Shell command history file | ```\.?(bash_|zsh_|sh_|z)+history``` |
| MySQL client command history file | ```(\.)?mysql_history``` |
| PostgreSQL client command history file | ```(\.)?psql_history``` |
| PostgreSQL password file | ```(\.)?pgpass``` |
| Ruby IRB console history file | ```(\.)?irb_history```|
| Pidgin chat client account configuration file | ```\.?purple/accounts\.xml``` |
| Hexchat/XChat IRC client server list configuration file | ```\.?xchat2?/servlist.conf``` |
| Irssi IRC client configuration file | ```\.?irssi/config``` |
| Recon-ng web reconnaissance framework API key database | ```\.?recon-ng/keys\.db``` |
| DBeaver SQL database manager configuration file | ```\.?dbeaver-data-sources(-[0-9]+)?\.xml``` |
| Mutt e-mail client configuration file | ```\.?muttrc``` |
| S3cmd configuration file | ```\.?s3cfg``` |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |

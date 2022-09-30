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

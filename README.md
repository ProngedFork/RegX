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

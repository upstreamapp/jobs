# Software Developer

- [About Upstream](#about-upstream)
- [About this Role](#about-this-role)
- [About You](#about-you)
- [Ready to Apply?](#ready-to-apply)

## About Upstream

**Upstream** is building the place for your professional social life: a platform where professionals can get help & help others, meet people in fun live video mixer events, and build a community of like-minded professionals.

## About this Role

We are looking to hire a full-stack engineer to join our team & focus on building the web-facing interface of our platform. Our mobile iOS & Android apps are already actively used by thousands of people, and we'd like to fill the gap and bring the same great experience to the browser.

**Our tech** is built mostly on {Type,Java}Script. Our servers are all running Kubernetes on AWS's EKS. We utilize PSQL, Elasticsearch, and Redis for our storage and caching. Everything we ship gets profiled and performance monitored using tools like Telegraf, Grafana, and InfluxDB.

**Remote work** is built into Upstream's DNA. Our team is spread across the US, and you'll be able to work from anywhere you'd like within the country, so good communication skills will come in handy. Our company offers unlimited vacation days, in addition to full benefits, including health, dental, and vision coverage.

## About You

**You** are a self-starter, self-motivating developer who can take an idea and run independently. You love seeing a project go from ideation to fruition. While your focus will be on our front-end client, you'll undoubtedly be making changes to our API server, infrastructure, and tooling. We'd like you to:

- Have at least 4 years of experience writing code, in any language
- Have an understanding of {server, client}-side performance, and how to measure and optimize it
- Write {some unit, but mostly integration} tests
- Have contributed to open-source projects

## Ready to Apply?

Send a POST request (`content-type` can be JSON, or multipart if including a file) to our jobs API endpoint, along with your information:

Endpoint: `https://api.upstreamapp.com/jobs`

| Param     | Description          | Required |
| --------- | -------------------- | -------- |
| email     | Email Address        | T        |
| firstName | First Name           | T        |
| lastName  | Last Name            | T        |
| phone     | Phone Number         | F        |
| linkedIn  | LinkedIn ID (or URL) | F        |
| twitter   | Twitter Handle       | F        |
| github    | Github Username      | F        |
| resume    | Resume File          | F        |

Your request might end up looking similar to this:

```bash
curl \
  -X POST \
  -H "Content-Type: multipart/form-data" \
  -F "email=annie@upstreamapp.com" \
  -F "firstName=Annie" \
  -F "lastName=Dogg" \
  -F "github=schonfeld" \
  -F "resume=@/home/annie/Desktop/resume.pdf" \
  https://api.upstreamapp.com/jobs
```

Alternatively, simply send an email to [michael@upstreamapp.com](michael@upstreamapp.com). Attach your resume, links, or recent pictures of your cute fluffy dog (cats are okay, too).

# Documentation about SciCrop jobs API

- In order to post your resume to a job offer at SciCrop, please use the url: https://engine.scicrop.com/scicrop-engine-web/api/v1/jobs/post_resume , with a **POST** method, **application/json content-type** and your resumè as a **json object**, in the POST body.
- The resumè must be sent as a **json object**, with **ALL** keys filled with valid values.
- Note that all dates must be expressed as **numeric type** in **Unix epoch** standard.
- Note that *degrees, programming_skills, database_skills* and *hobbies* are arrays.
- A correct response is expressed by **HTTP 200** code, as well as a confirmation email, with an invite to an interview.

### Resume JSON object example:

```js
{
	"full_name": "Robinson Crusoe",
	"email": "robinson@crusoe.com",
	"mobile_phone": "+55 (55) 555-555-555",
	"age": 20,
	"home_address": "101 Jungle Ave, Trinidad Island",
	"start_date": 1573077739,
	"opportunity_tag": "dev_intern_200",
	"past_jobs_experience": "I worked as a sailor on fishing vessels. Took care of deck maintenance and cleaning for 3 years on 7 seas.",
	"degrees": [{
		"institution_name": "Sea University",
		"degree_name": "Sailing School",
		"begin_date": 1514764800,
		"end_date": 1640995200
	}],
	"programming_skills": ["python", "java", "go"],
	"database_skills": ["mysql", "postgresql"],
	"hobbies": ["fishing", "wood carving"],
	"why": "After living 28 years all alone in an un‐inhabited Island, I've built a strong experience to join the SciCrop ship, into a new journey.",
	"git_url_repositories": "https://github.com/robinson_crusoe"
}
```

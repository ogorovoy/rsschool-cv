# Oleg Gorovoy

<img src="https://github.com/ogorovoy/rsschool-cv/blob/main/me.jpeg" width="150" style="float: right; margin-left: 20px;">

## Contacts:
- Email: xxx@gmail.com
- Phone number:  xxx-xxx-936
- LinkedIn: http://linkedin.com/in/oleg-gorovoy-5865aa100

Personal data is anonymized in accordance with the GDPR. 
Hopefully enough accounts on LinkedIn

## About me:
I am 33 years old and have been living in Germany for many years. You can find more information on my LinkedIn profile.
My passion for IT started many years ago. My first job was in technical support for computers and other devices. Then I worked as a system administrator in E-Commerce for two years. Currently, I am involved in software testing.
Although JS was not previously part of my responsibilities and I know it on the surface, I decided to expand my employment competencies to remain in demand and grow in my profession.



## Skills:
- Splunk / Grafana
- Java / Python
- PHP 
- Powershell / Windows register
- Git / GitLab
- Pipelines / Runners / Airflow
- MS Office 365
- Jira / Confluence
- SQL
- Docker
- Zabbix
etc.

## Project Examples:
- **[CV](https://github.com/ogorovoy/rsschool-cv)**
- **[CO2](https://github.com/ogorovoy/CO2/)**

## Code Example:
**No Name Project**
```
url = 'https://app.rs.school/course/score?course=js-fe-preschool-2024q2'
driver.get(url)
time.sleep(3)

login_button = driver.find_element(By.XPATH, '/html/body/div/main/div/div[2]/ul/li/span/button').click()
time.sleep(5)
login_input = driver.find_element(By.ID, 'login_field').send_keys(login)
password_field = driver.find_element(By.ID, 'password').send_keys(password)
sign_in = driver.find_element(By.XPATH, '/html/body/div[1]/div[3]/main/div/div[3]/form/div/input[13]').click()
time.sleep(10)

def extract_github_links():
    soup = BeautifulSoup(driver.page_source, 'html.parser')
    links = [link['href'] for link in soup.find_all('a', href=True) if link['href'].startswith('https://github.com/')]
    return links

all_github_links = []

for page in pages(1, 47):
    page_link_xpath = f"//a[@rel='nofollow' and text()='{page}']"
    try:
        page_link = driver.find_element(By.XPATH, page_link_xpath).click()
        time.sleep(5)
        all_github_links.extend(extract_github_links())
    except Exception as e:
        print(f"not found link to page nr {page}: {e}")
        continue
data_file = 'data.csv'
df = pd.DataFrame(all_github_links, columns=['GitHub Links'])
df.to_csv(data_file, index=False)

```


## Education:
WSB Merito Wroclaw - Internal Security






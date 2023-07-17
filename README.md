Доброго времени. Помоги пожалуйста со вторым заданием по Grafana. Я уперся в стенку и не понимаю как дальше действововать!

Создать организацию в GitLab.

Подсказка: зарегистрируетесь в GitLab. Для настройки орагнизации воспользуйтесь соответствующим разделом документации.

Включить и настроить GitLab Auth в конфигурациях grafanа.ini.

Подсказка: конфигурационный файл по умолчанию располагается в /etc/grafana/grafana.ini.

Проверить работу внешнего провайдера авторизации.

Подсказка: не забудьте сменить параметр root_url в конфиг-файле Grafana для корректной работы обратного редиректа после авторизации в GitLab.


Настройки 


№root_url = http://206.189.110.226:3000/login/gitlab


#################################### GitLab Auth #########################
[auth.gitlab]
enabled = true
allow_sign_up = true
client_id = 8bbbb1767d3cf0a2d0c6feb92807bf985ad257a34c8b5f32cae49a0dd281e27c
client_secret = 5ff8d5571460cbe78dd57c9f50d18e690bd8945e707ffabe2f09b606bc2bd759
scopes = api
auth_url = https://gitlab.com/oauth/authorize
token_url = https://gitlab.com/oauth/token
api_url = https://gitlab.com/api/v4
№allowed_domains =
№allowed_groups =
###############################################################################
я взял client_id, client_secret в user settings - Aplication 
Application: testesdddd
Application ID	8bbbb1767d3cf0a2d0c6feb92807bf985ad257a34c8b5f32cae49a0dd281e27c
Secret	5ff8d5571460cbe78dd57c9f50d18e690bd8945e707ffabe2f09b606bc2bd759
Callback URL	http://206.189.110.226:3000/login/gitlab

Scopes	
api (Access the authenticated user's API)
read_api (Read Api)
read_user (Read the authenticated user's personal information)
create_runner (Grants create access to the runners)
read_repository (Allows read-only access to the repository)
write_repository (Allows read-write access to the repository)
read_registry (Grants permission to read container registry images)
read_observability (Allows read-only access to GitLab Observability)
write_observability (Allows read-write access to GitLab Observability)
sudo (Perform API actions as any user in the system)
admin_mode (Admin Mode is a functionality designed to limit the access level of administrator's personal access tokens.)
openid (Authenticate using OpenID Connect)
profile (Allows read-only access to the user's personal information using OpenID Connect)
email (Allows read-only access to the user's primary email address using OpenID Connect)
При переходе на Callback URL	http://206.189.110.226:3000/login/gitlab Я получаю ошибку 

An error has occurred
The redirect URI included is not valid.


№В чем может быть причина?

# Данные отправляемые на tsend.php
Данные отправляются POST запросом.
## special_coupon_form
Отключает примечание о повторной заявке
Отключает проверку на дубли сделки
> special_coupon_form=1
## disable_force_forward_lead
Отключает настройку "Движение сделки только вперед" при необходимости смены этапа сделки.
> disable_force_forward_lead=1
## modify_ctime_lead
Дата создания сделки в UNIX. Работает только для создания сделки.
> modify_ctime_lead=1625730224
## no_action_if_found
Ничего не делать, если нашли дубль сделки.
> no_action_if_found=1
## phone
Номер телефона клиента
> phone=+79991112233 (в любом формате)
## email
Email клиента
> email=notify@mail.ru
## name
Имя клиента
## status_id
id этапа сделки
> По умолчанию: 26763700 (Поступила заявка)
> Если передан form_name, id этапа сделки может измениться, даже если передан status_id
## form_name
Название формы
| Название формы | Статус ID | Статус | Проверка на дубли | Примечание повт. заявки | Менять статус сделки
|----|:---:|:-----------:|--|------|------|
| mailing | - | - | + | + | - | 
| lk_without_article | 26763838| Получена статья | - | + | - |
| lk_with_article | 26763700 |  | - | + | - |
| form_activate_promo_code_2 | 26763700 | Поступила заявка | + | - | + |
| form_submit_application_2 | 26763700 | Поступила заявка | + | - | + |
| form_get_consultation_2 | 26763700 | Поступила заявка | + | - | + |
| activate_promo_code_2 | 26763700 | Поступила заявка | + | - | + |
| get_consultation_2 | 26763700 | Поступила заявка | + | - | + |
| submit_application_2 | 26763700 | Поступила заявка | + | - | + |
| form_activate_promo_code_3 | 26763703 | Написали сообщение | + | - | + |
| form_submit_application_3 | 26763703 | Написали сообщение | + | - | + |
| form_get_consultation_3 | 26763703 | Написали сообщение | + | - | + |
| activate_promo_code_3 | 26763703 | Написали сообщение | + | - | + |
| submit_application_3 | 26763703 | Написали сообщение | + | - | + |
| get_consultation_3 | 26763703 | Написали сообщение | + | - | + |
| form_activate_promo_code_4 | 26763838 | Получена статья | + | - | + |
| form_submit_application_4 | 26763838 | Получена статья | + | - | + |
| form_get_consultation_4 | 26763838 | Получена статья | + | - | + |
| activate_promo_code_4 | 26763838 | Получена статья | + | - | + |
| submit_application_4 | 26763838 | Получена статья | + | - | + |
| get_consultation_4 | 26763838 | Получена статья | + | - | + |

| Название формы | Статус ID | Статус | Проверка на дубли | Примечание повт. заявки | Менять статус сделки
|----|:---:|:-----------:|--|------|------|
| free_audit_1 | 26763838 | Получена статья | + | + | + |
| quiz_1_4 | 26763838 | Получена статья | + | + | + |
| quiz_2_4 | 26763838 | Получена статья | + | + | + |
| discuss_task_3 | 26763838 | Получена статья | + | + | + |
| find_cost_4 | 26763838 | Получена статья | + | + | + |
| submit_application_4 | 26763838 | Получена статья | + | + | + |
| activate_promo_code_4 | 26763838 | Получена статья | + | + | + |
| find_dedline_4 | 26763838 | Получена статья | + | + | + |
| warranty_3 | 26763838 | Получена статья | + | + | + |
> Если проверка на дубли не ведется, то создается новая сделка.

## host
hostname
>host=worldscipubl.com
## questions
Квиз (Идет в примечание)
>questions=Текст
## other_fields
Предпочитительный способ связи (Идет в примечание)
>other_fields=Текст
## friend_id
>friend_id=val
## partner_program
>partner_program=val
## coupon
>coupon=val
## discount_coupon
>discount_coupon=val
## token
>token=val
## date
>date=val
## vuz_name
>vuz_name=val
## country
>country=val
## article_title
>article_title=val
## wishes_journal
>wishes_journal=val
## order_id
>order_id=val
## post
profession
>post=val
## cookie - в формате JSON 

> JSON
> {\"_uc_utm_source\":\"val\",\"_uc_utm_medium\":\"val\",\"_uc_utm_campaign\":\"val\",\"_uc_utm_content\":\"val\",\"_uc_utm_term\":\"val\",\"partner_id\":\"val\",\"roistat_visit\":\"val\"}
>> _uc_utm_source=val
> _uc_utm_medium=val
> _uc_utm_campaign=val
> _uc_utm_content=val
> _uc_utm_term=val
> partner_id=val
> roistat_visit=val

## before_note
> before_note=текст до начала основного примечания

## after_note
> after_note=текст после основного примечания

## override_note
> override_note=текст который заменит основное примечание
> отменяет before_note и after_note

## add_note
> add_note=текст дополнительного примечания



| Замечание | Исправление |
| :--- | :--- |
| В Task3.2 вместо успешного сценария записи с проверкой полиса, бронированием врача, оплатой и резервом LIS повторно приведён поток анализов. Перестрой sequence-диаграмму | /Task3/Task3_2/happy\_path\_sequence\_v2.puml |
| в таблице укажи три нужные компенсации: освобождение слота, возврат платежа и отмену резерва LIS | /Task3/Task3_2/compensation\_v2.md |
| Диаграмма Task2 названа C4 Level 2 и построена через Container, тогда как нужна контекстная C4 Level 1. | /Task3/Task2/TO\_BE\_v2.puml |
| Также согласуй противоречие: в Task2 для платежа указаны ретраи, а в Task4.1 они запрещены. | Типизоровал поведение в зависимости от ошибки. **/Task4/Task4\_1/task4\_1\_v2.md**  |
|В OpenAPI требуется GET /api/v1/appointments. Сейчас отсутствуют обязательные appointment_id, datetime и clinic_address, а BearerAuth объявлена, но не применена через security.| Убрано лишнее, исправлены ошибки, добавлены session_id и request_id. Вместо datetime - appointment_start и appointment_end. **/Task3/Task3\_3/appointments\_v2.yaml**|
|Блок безопасности стоит расширить: добавь mTLS между Gateway и сервисами, Retry-After для 429, certificate pinning и валидацию сертификатной цепочки. Для входа из мобильного приложения явно укажи Authorization Code Flow с PKCE.|/Task4/Task4\_3/|

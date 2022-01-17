#   Форматы сериализации

Основные задачи:

  - Хранение (тут желательно иметь восможность прочитать произвольный кусок)
  - Передача (компактность)
  - Обработка (в основном, редактируемость)
  - Эволюция и совместимость реализаций (разные люди будут писать на разных языках и разных версиях)

1. Текстовые форматы
    1. классический Key: Value в HTTP, SMTP итд
       https://datatracker.ietf.org/doc/html/rfc2616#section-10.4.9
    2. XML etc
       https://developer.mozilla.org/en-US/docs/Web/XML/XML_introduction
    3. JSON https://www.json.org/json-en.html
       неоднозначности JSON: Parsing JSON is a Minefield http://seriot.ch/projects/parsing_json.html
    4. Ragel, генератор парсеров текстовых форматов http://www.colm.net/open-source/ragel/ Баг Cloudbleed: https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/
2. Двоичные
    1. Protobuf набор примитивов https://developers.google.com/protocol-buffers/docs/overview#scalar
    сага о LEB128 https://developers.google.com/protocol-buffers/docs/encoding#structure
    2. Thrift
    3. Cap’n Proto https://capnproto.org
    4. FlatBuffers работа над ошибками от Google https://google.github.io/flatbuffers/flatbuffers_internals.html
3. Гарри Поттер и кошмары Unicode
    1. карта BMP https://unicode.org/roadmaps/bmp/
    2. статистика по исользованию не-BMP в реале http://replicated.cc/concepts/unicode (примерно 0 до emoji, чуть больше теперь)

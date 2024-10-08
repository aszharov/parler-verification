# Результаты работы с моделью parler-tts-mini-jenny-30h

Поскольку датасет модели не был разделён на train / test, свою оценку модели я проводил без его использования, чтобы посмотреть, как она работает на незнакомых промптах и описаниях. Промпты были придуманы, описания с особенностями голоса и звука были собраны по образу и подобию, представленных авторами модели [parler-tts](https://www.text-description-to-speech.com/). В ряде случаев модель не проводит генерацию. Все результаты представлены внутри ноутбука. Наиболее важные из них:
- Прослеживается тренд повышения высоты голоса при изменении описания к промпту от very low-pitched voice до very high-pitched voice (фундаментальная частота от 196.9 до 236.6 Гц);
- Прослеживается тренд повышения скорости речи при изменении описания к промпту от very slowly до very quickly (от 8.8 до 13.9 фонем в секунду);
- Невозможно говорить о какой-либо чувствительности модели к изменениям в описании промпта в случае добавления шума или эха;
- Большая часть генераций выполнена успешно с точки зрения корректности и разборчивости (медианное значение WER на 240 промптах 0.08);
- Доля успешных генераций - 82%.

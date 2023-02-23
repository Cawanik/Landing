<template>
  <v-container>
    <v-row>
      <v-col md="6" sm="12" cols="12">
        <v-card :dark="false" color="#4E415B" class="card__background">
          <div class="card__numeric">1</div>
          <v-card-title>Наставничество</v-card-title>
          <v-card-subtitle>по договоренности</v-card-subtitle>
          <p class="card__text">
            Индивидуальное наставничество по таргету в вк.<br>
            Если вы хотите освоить новую онлайн специальность, стать уверенным таргетологом и делать крутые результаты
            своим
            клиентам, а может просто улучшить свои знания в маркетинге и таргетинге, то приглашаю к себе на
            наставничество.<br>
            Программа наставничества (можно выбрать индивидуально темы, которые вам нужны):
          </p>
          <ul>
            <li>Как оформить продающую группу, выстраивание воронки продаж</li>
            <li>Какие посты писать для вк</li>
            <li>Контентные воронки в постах</li>
            <li>Анализ ца по лестнице Бенна ханта + как анализировать аудиторию, где ее искать</li>
            <li>Готовые схемы анализа ца</li>
            <li>Как составить стратегии, воронки продаж, которые будут работать...</li>

          </ul>
          <v-card-actions class="card__actions">
            <v-btn width="100%" color="#B1BEA4" link href="">Читать далее...</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col md="6" sm="12" cols="12">
        <v-card :dark="false" color="#4E415B" class="card__background">
          <div class="card__numeric">2</div>
          <v-card-title>Настройка таргетированной рекламы</v-card-title>
          <v-card-subtitle>от 12 000 ₽</v-card-subtitle>
          <p class="card__text">
            Если у вас мало клиентов, боитесь, что однажды придется закрывать ваш бизнес или стоите на одном уровне
            дохода и не можете его повысить, то я смогу вам помочь!
            <br>
            Каждый 2 клиент возвращается ко мне, чтобы продолжить продвигаться еще раз, потому что у него повышается
            доход в несколько раз, и он знает, что сможет увеличить его еще вместе со мной. Ведь подписчики с рекламы
            покупают продукты еще несколько лет.
            <br>
            Я уже 4 года развиваюсь в сфере маркетинга, прошла курсы копирайтинга, дизайна, сторисмейкерства, визуала,
            продаж. И продолжаю изучать что-то новое, чтобы добиваться еще лучших результатов и помогать своим клиентам
            комплексно улучшать бизнес...
          </p>
          <v-card-actions class="card__actions">
            <v-btn width="100%" color="#B1BEA4" link href="">Читать далее...</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col md="6" sm="12" cols="12">
        <v-card :dark="false" color="#4E415B" class="card__background">
          <div class="card__numeric">3</div>
          <v-card-title>Консультация</v-card-title>
          <v-card-subtitle>от 2 500 ₽</v-card-subtitle>
          <p class="card__text">
            Если у вас есть пробелы в рекламе вконтакте:
          </p>
          <ul>
            <li>нет заявок с рекламы</li>
            <li>не идут подписчики</li>
            <li>мало переходов</li>
            <li>боитесь, что просто сливаете деньги клиента зря</li>
            <li>не знаете, как создать рекламное объявление, которое зацепит</li>
            <li>вроде все делаете правильно, но статистика объявления не устраивает</li>
            <li>вы запустили рекламу на себя, но не получили заявок</li>
          </ul>
          <p class="card__text">
            ТО обращайтесь за часовой консультацией, где мы разберем ваш рекламный кабинет...
          </p>
          <v-card-actions class="card__actions">
            <v-btn width="100%" color="#B1BEA4" link href="">Читать далее...</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col md="6" sm="12" cols="12">
        <v-card :dark="false" color="#4E415B" class="card__background">
          <div class="card__numeric">4</div>
          <v-card-title>Распаковка личности</v-card-title>
          <v-card-subtitle>от 3 000 ₽</v-card-subtitle>
          <p class="card__text">
            Если у вас проблемы с ведением своего блога и вы не знаете:
          </p>
          <ul>
            <li>о чем говорить в сторис, чтобы продать вашу услугу без навязывания</li>
            <li>у вас есть страхи и сомнения по поводу ведения блога</li>
            <li>не знаете, как начать выходить в истории</li>
            <li>вам кажется, что вы неинтересный и вам нечего рассказывать</li>
            <li>у вас каша в голове, не знаете, как себя позиционировать</li>
          </ul>
          <p class="card__text">
            То предлагаю вам распаковку личности, в ходе которой мы раскроем вас и ваши страхи, поговорим о том, что и как рассказывать в историях, как продать лучше вашу услугу...
          </p>
          <v-card-actions class="card__actions">
            <v-btn width="100%" color="#B1BEA4" link href="">Читать далее...</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Services"
}
</script>

<style lang="scss" scoped>
.card {
  &__background{
    overflow: hidden;
    max-height: 700px;
    min-height: 700px;
    @media screen and (max-width: 960px){
      max-height: 800px;
      min-height: 800px;
    }
  }
  &__actions {
    position: absolute;
    bottom: 0;
    width: 100%;
  }

  &__numeric {
    z-index: 0;
    height: 0;
    color: #3C3541;
    font-size: 250px;
    text-align: right;
    line-height: 100%;
    right: 0;
  }

  &__text {
    z-index: 1;
    padding: 16px;
    color: white;
    font-size: 16px;
    line-height: 150%;
  }

  .v-btn {
    width: 100%;
    padding-left: 20px;
    padding-bottom: 20px;
  }
}

ul {
  margin-left: 20px;
  margin-bottom: 20px;
}
</style>

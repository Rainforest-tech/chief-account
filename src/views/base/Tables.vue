<template>
  <h2 align="middle">Критерии трудового вклада 2022</h2>
  <CTable style="" align="middle" bordered hover responsive>
    <CTableHead align="middle">
      <CTableRow align="middle">
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >№</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Показатель</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Каскадирование</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Порядок расчета</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Владелец процесса</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Ед. изм.</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Вес</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >План</CTableHeaderCell
        >
        <CTableHeaderCell style="background-color: #ffcc5c" scope="col"
          >Ожид</CTableHeaderCell
        >
      </CTableRow>
    </CTableHead>
    <CTableBody>
      <CTableRow style="text-align: center"
        ><CTableDataCell colspan="9">
          обязательные базовые показатели производственных СП</CTableDataCell
        ></CTableRow
      >
      <CTableRow responsive>
        <CTableHeaderCell scope="row">1</CTableHeaderCell>
        <CTableDataCell color="light"
          >Выполнение плана выручки собственными силами СП в соответствии с утв.
          БП (УИУ ПИР)</CTableDataCell
        >
        <CTableDataCell>КПЭ ГД</CTableDataCell>
        <CTableDataCell
          >Расчет осуществляется за вычетом внутреннего распределения
          (допускается нормализация по согласованию в ПАО "НК "Роснефть")
          Выполнение утвержденного БП ниже 95% - показатель = 0 Выполнение
          утвержденного БП на 95 - 99,9% - Кф=0,5 Выполнение утвержденного БП на
          100 - 105% - Кф=1 Выполнение утвержденного БП на 105,1% и выше -
          линейный расчет показателя 105 + (Выполнение - 105)*2 При нормализации
          не допускается превышение 100% выполнения
        </CTableDataCell>
        <CTableDataCell>ФЭУ</CTableDataCell>
        <CTableDataCell>млн. руб.</CTableDataCell>
        <CTableDataCell color="light">25</CTableDataCell>
        <CTableDataCell color="light">75,000</CTableDataCell>
        <CTableDataCell>75,000</CTableDataCell>
      </CTableRow>
      <CTableRow align="middle">
        <CTableHeaderCell scope="row">2</CTableHeaderCell>
        <CTableDataCell color="light"
          >Повышение качества работ и услуг блок ПИР в целом</CTableDataCell
        >
        <CTableDataCell>КПЭ ГД</CTableDataCell>
        <CTableDataCell
          >Расчет осуществляется на основании среднегодовой оценки качества
          работ и официальных оценок качества Наличие формализованных претензий
          государственных органов и ТТЭС Компании - показатель = 0 Среднегодовая
          оценка качества 6,2 - показатель = 0 Среднегодовая оценка качества 6,2
          - 6,9 - Кф=0,5 Среднегодовая оценка качества 6,91 - 7,2 - Кф=1
          Среднегодовая оценка качества 7,21 и более - линейный расчет
          показателя 100+(Оценка-8,2)*20</CTableDataCell
        >
        <CTableDataCell>Отдел СМК</CTableDataCell>
        <CTableDataCell>балл</CTableDataCell>
        <CTableDataCell color="light">15</CTableDataCell>
        <CTableDataCell color="light">8.2</CTableDataCell>
        <CTableDataCell>8.2</CTableDataCell>
      </CTableRow>
      <CTableRow
        ><CTableDataCell colspan="9" style="text-align: center">
          показатели производственных СП</CTableDataCell
        ></CTableRow
      >
      <CTableRow align="middle">
        <CTableHeaderCell scope="row">3</CTableHeaderCell>
        <CTableDataCell color="success"
          >Внедрение в производственно-хозяйственную деятельность
          рационализаторских решений и прочих предложений, приводящих к
          улучшению качества продукции (услуг)</CTableDataCell
        >
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell
          >Заключение новых договоров и выполнение ПИР по объектам
          Харампурнефтегаз, Пурнефтегаз Договоры по объектам Харампурнефтегаз,
          Пурнефтегаз заключены - Кф=1 Заключен один из договоров - Кф=0,5
          Договоры по объектам Харампурнефтегаз, Пурнефтегаз не заключены - Кф=0
        </CTableDataCell>
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell>%</CTableDataCell>
        <CTableDataCell color="light">15</CTableDataCell>
        <CTableDataCell color="light">100</CTableDataCell>
        <CTableDataCell>100</CTableDataCell>
      </CTableRow>
      <CTableRow align="middle">
        <CTableHeaderCell scope="row">4</CTableHeaderCell>
        <CTableDataCell color="success"
          >Оперативность обеспечения объектов строительства техническими
          решениями</CTableDataCell
        >
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell>
          Повышение оперативности выдачи технических решений и отработки
          вопросов в части сопровождения СМР (выдача втечение 10 рабочих дней),
          отсутствие обоснованных претензий со стороны Заказчиков.
        </CTableDataCell>
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell>%</CTableDataCell>
        <CTableDataCell color="light">15</CTableDataCell>
        <CTableDataCell color="light">100</CTableDataCell>
        <CTableDataCell>100</CTableDataCell>
      </CTableRow>
      <CTableRow align="middle">
        <CTableHeaderCell scope="row">5</CTableHeaderCell>
        <CTableDataCell color="success"
          >Организация работы по сопровождению СМР</CTableDataCell
        >
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell
          >Внедрение в производственно-хозяйственную деятельность
          рационализаторских решений и прочих предложений, приводящих к
          улучшению качества продукции (услуг)
        </CTableDataCell>
        <CTableDataCell>ГИ</CTableDataCell>
        <CTableDataCell>балл</CTableDataCell>
        <CTableDataCell color="light">10</CTableDataCell>
        <CTableDataCell color="light">1</CTableDataCell>
        <CTableDataCell>1</CTableDataCell>
      </CTableRow>
      <CTableRow
        ><CTableDataCell colspan="9" style="text-align: center">
          показатели, обеспечивающие научно-техническое и управленческое
          развитие ТННЦ и Компании</CTableDataCell
        ></CTableRow
      >
      <CTableRow align="middle">
        <CTableHeaderCell scope="row">6</CTableHeaderCell>
        <CTableDataCell color="light"
          >Выполнение комплексного показателя развития научно-технического
          потенциала СП, безопасность труда</CTableDataCell
        >
        <CTableDataCell>Рейтинг, стратегия ТННЦ</CTableDataCell>
        <CTableDataCell
          ><CTableRow style="text: center">Комплексный показатель</CTableRow>
          <hr />
          <CTableRow style="text: center"
            >К1 Выполнение ССЧ по блоку ПИР за 2022 год показатель не выполнен,
            коэффициент 0 - выполнение ССЧ ниже 95% показатель выполнен
            частично, коэффициент 0,5 - выполнение ССЧ на 95 - 98% показатель
            выполнен, коэффициент 1 - выполнение ССЧ на 98,1-100% выполнение ССЧ
            более чем на 100,1% - линейный расчет 100 + процент
            перевыполнения</CTableRow
          >
          <hr />
          <CTableRow style="text: center"
            >К2 Внутренняя автоматизация блока ПИР: показатель выполнен,
            коэффициент - 1: - реализация формы реестров ИУ и АН для
            планирования и мониторинга выполнения работ по запросам; -
            реализация формы "Планы заказчиков" для хранения версий ф.9.4 ОГ,
            выполнения анализа; - реализация формы для формирования РПЗ, МЗ по
            направлению ПИР, проработка модуля мониторинга закупочных процедур
            показатель выполнен частично, коэффициент - 0,6: - реализация формы
            реестров ИУ и АН для планирования и мониторинга выполнения работ по
            запросам; - реализация формы "Планы заказчиков" для хранения версий
            ф.9.4 ОГ, выполнения анализа; показатель выполнен частично,
            коэффициент - 0,3: - реализация формы реестров ИУ и АН для
            планирования и мониторинга выполнения работ по запросам; показатель
            не выполнен, коэффициент 0 - не выполнен ни один из вышеназванных
            пунктов показатель перевыполнен, коэффициент - 1,2 - реализация
            дополнительных к вышеназванным пунктов утвержденного Плана
            автоматизации
          </CTableRow>
          <hr />
          <CTableRow style="text: center"
            >К3 Производственный травматизм: отсутствие травм на производстве -
            показатель выполнен, коэффициент - 1 наличие травм на производстве -
            показатель не выполнен, коэффициент - 0</CTableRow
          >
        </CTableDataCell>
        <CTableDataCell>Управление по персоналу, УРИТ, ПБОТОС</CTableDataCell>
        <CTableDataCell
          ><div :class="$store.state.sidebarVisible ? 'pos-one' : 'pos-seven'">
            x
          </div>
          <hr :class="$store.state.sidebarVisible ? 'pos-two' : 'pos-eight'" />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-three' : 'pos-nine'"
            >%</CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-four' : 'pos-ten'" />
          <CTableRow>балл</CTableRow>
          <hr
            :class="$store.state.sidebarVisible ? 'pos-five' : 'pos-eleven'"
          />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-six' : 'pos-twelve'"
            >балл</CTableRow
          >
        </CTableDataCell>
        <CTableDataCell>
          <CTableRow color="light"
            ><div
              :class="$store.state.sidebarVisible ? 'pos-one' : 'pos-seven'"
            >
              20
            </div></CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-two' : 'pos-eight'" />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-three' : 'pos-nine'"
            >30</CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-four' : 'pos-ten'" />
          <CTableRow>30</CTableRow>
          <hr
            :class="$store.state.sidebarVisible ? 'pos-five' : 'pos-eleven'"
          />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-six' : 'pos-twelve'"
            >40</CTableRow
          >
        </CTableDataCell>
        <CTableDataCell>
          <CTableRow color="light"
            ><div
              :class="$store.state.sidebarVisible ? 'pos-one' : 'pos-seven'"
            >
              x
            </div></CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-two' : 'pos-eight'" />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-three' : 'pos-nine'"
            >182</CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-four' : 'pos-ten'" />
          <CTableRow>1</CTableRow>
          <hr
            :class="$store.state.sidebarVisible ? 'pos-five' : 'pos-eleven'"
          />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-six' : 'pos-twelve'"
            >1</CTableRow
          >
        </CTableDataCell>
        <CTableDataCell>
          <CTableRow color="light"
            ><div
              :class="$store.state.sidebarVisible ? 'pos-one' : 'pos-seven'"
            >
              x
            </div></CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-two' : 'pos-eight'" />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-three' : 'pos-nine'"
            >182</CTableRow
          >
          <hr :class="$store.state.sidebarVisible ? 'pos-four' : 'pos-ten'" />
          <CTableRow>1</CTableRow>
          <hr
            :class="$store.state.sidebarVisible ? 'pos-five' : 'pos-eleven'"
          />
          <CTableRow
            :class="$store.state.sidebarVisible ? 'pos-six' : 'pos-twelve'"
            >1</CTableRow
          >
        </CTableDataCell>
      </CTableRow>
      <CTableRow>
        <CTableDataCell
          style="text-align: right; background-color: #ffcc5c"
          colspan="6"
          >Итого</CTableDataCell
        >
        <CTableDataCell style="background-color: #ffcc5c">100</CTableDataCell>
        <CTableDataCell style="background-color: #ffcc5c" colspan="2"
          >X</CTableDataCell
        >
      </CTableRow>
    </CTableBody>
  </CTable>
</template>

<script>
export default {
  name: 'Tables',
}
</script>

<style lang="scss" scoped>
@media (min-width: 1200px) {
  .pos-one {
    position: relative !important;
    bottom: 285px;
    text-align: center;
  }
}
.pos-two {
  position: relative !important;
  bottom: 290px;
  text-align: center;
}
.pos-three {
  position: relative !important;
  bottom: 220px;
  text-align: center;
}
.pos-four {
  position: relative !important;
  bottom: 170px;
  text-align: center;
}
.pos-five {
  position: relative !important;
  top: 215px;
  text-align: center;
}
.pos-six {
  position: relative !important;
  top: 250px;
  text-align: center;
}
.pos-seven {
  position: relative !important;
  bottom: 280px;
  text-align: center;
}
.pos-eight {
  position: relative !important;
  bottom: 285px;
  text-align: center;
}
.pos-nine {
  position: relative !important;
  bottom: 225px;
  text-align: center;
}
.pos-ten {
  position: relative !important;
  bottom: 170px;
  text-align: center;
}
.pos-eleven {
  position: relative !important;
  top: 215px;
  text-align: center;
}
.pos-twelve {
  position: relative !important;
  top: 235px;
  text-align: center;
}
</style>

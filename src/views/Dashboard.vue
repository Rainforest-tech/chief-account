<template>
  <div>
    <WidgetsStatsA />
    <CRow>
      <CCol :md="12">
        <CCard class="mb-4">
          <CCardBody>
            <CRow>
              <CCol :sm="5">
                <h4 id="traffic" class="card-title mb-0">
                  Ключевые показатели
                </h4>
                <div class="small text-medium-emphasis">Январь 2021</div>
              </CCol>
              <CCol :sm="7" class="d-none d-md-block">
                <CButton color="primary" class="float-end">
                  <CIcon icon="cil-cloud-download" />
                </CButton>
                <CButtonGroup
                  class="float-end me-3"
                  role="group"
                  aria-label="Basic outlined example"
                >
                  <CButton color="secondary" variant="outline">День</CButton>
                  <CButton color="secondary" variant="outline" active
                    >Месяц</CButton
                  >
                  <CButton color="secondary" variant="outline">Год</CButton>
                </CButtonGroup>
              </CCol>
            </CRow>
            <CRow>
              <MainChartExample
                style="height: 300px; max-height: 300px; margin-top: 40px"
              />
            </CRow>
          </CCardBody>
          <CCardFooter>
            <CRow :xs="{ cols: 1 }" :md="{ cols: 5 }" class="text-center">
              <CCol class="mb-sm-2 mb-0">
                <div class="text-medium-emphasis">Факт</div>
                <strong>29.703 единиц (40%)</strong>
                <CProgress
                  class="mt-2"
                  color="success"
                  thin
                  :precision="1"
                  :value="40"
                />
              </CCol>
              <CCol class="mb-sm-2 mb-0 d-md-down-none">
                <div class="text-medium-emphasis">Текущий</div>
                <strong>24.093 единиц (20%)</strong>
                <CProgress
                  class="mt-2"
                  color="info"
                  thin
                  :precision="1"
                  :value="20"
                />
              </CCol>
              <CCol class="mb-sm-2 mb-0">
                <div class="text-medium-emphasis">Прогноз</div>
                <strong>78.706 единиц (60%)</strong>
                <CProgress
                  class="mt-2"
                  color="warning"
                  thin
                  :precision="1"
                  :value="60"
                />
              </CCol>
              <CCol class="mb-sm-2 mb-0">
                <div class="text-medium-emphasis">План</div>
                <strong>22.123 единиц (80%)</strong>
                <CProgress
                  class="mt-2"
                  color="danger"
                  thin
                  :precision="1"
                  :value="80"
                />
              </CCol>
              <CCol class="mb-sm-2 mb-0 d-md-down-none">
                <div class="text-medium-emphasis">Средний показатель</div>
                <strong>25.000 единиц (40.15%)</strong>
                <CProgress class="mt-2" :value="40" thin :precision="1" />
              </CCol>
            </CRow>
          </CCardFooter>
        </CCard>
      </CCol>
    </CRow>

    <br />
    <CTable align="middle" class="mb-0 border" hover responsive>
      <CTableHead color="light">
        <CTableRow>
          <CTableHeaderCell class="text-center">
            <CIcon name="cil-people" />
          </CTableHeaderCell>
          <CTableHeaderCell>Пользователь</CTableHeaderCell>
          <CTableHeaderCell class="text-center">Отдел</CTableHeaderCell>
          <CTableHeaderCell>Использование</CTableHeaderCell>

          <CTableHeaderCell>Активность</CTableHeaderCell>
        </CTableRow>
      </CTableHead>
      <CTableBody>
        <CTableRow v-for="item in tableExample" :key="item.name">
          <CTableDataCell class="text-center">
            <CAvatar
              size="md"
              :src="item.avatar.src"
              :status="item.avatar.status"
            />
          </CTableDataCell>
          <CTableDataCell>
            <div>{{ item.user.name }}</div>
            <div class="small text-medium-emphasis">
              <span>{{ item.user.new ? 'Новый' : 'Текущий' }}</span> |
              {{ item.user.registered }}
            </div>
          </CTableDataCell>
          <CTableDataCell class="text-center">
            <CIcon size="xl" />
          </CTableDataCell>
          <CTableDataCell>
            <div class="clearfix">
              <div class="float-start">
                <strong>{{ item.usage.value }}%</strong>
              </div>
              <div class="float-end">
                <small class="text-medium-emphasis">
                  {{ item.usage.period }}
                </small>
              </div>
            </div>
            <CProgress
              thin
              :color="item.usage.color"
              :value="item.usage.value"
            />
          </CTableDataCell>

          <CTableDataCell>
            <div class="small text-medium-emphasis">Последний раз в сети</div>
            <strong>{{ item.activity }}</strong>
          </CTableDataCell>
        </CTableRow>
        <CTableRow> </CTableRow>
      </CTableBody>
    </CTable>
  </div>
</template>

<script>
import avatar1 from '@/assets/images/avatars/1.jpg'
import avatar2 from '@/assets/images/avatars/2.jpg'
import avatar3 from '@/assets/images/avatars/3.jpg'
import avatar4 from '@/assets/images/avatars/4.jpg'
import avatar5 from '@/assets/images/avatars/5.jpg'
import avatar6 from '@/assets/images/avatars/6.jpg'
import MainChartExample from './charts/MainChartExample'
import WidgetsStatsA from './widgets/WidgetsStatsTypeA.vue'

export default {
  name: 'Dashboard',
  components: {
    MainChartExample,
    WidgetsStatsA,
  },
  setup() {
    const progressGroupExample1 = [
      { title: 'Monday', value1: 34, value2: 78 },
      { title: 'Tuesday', value1: 56, value2: 94 },
      { title: 'Wednesday', value1: 12, value2: 67 },
      { title: 'Thursday', value1: 43, value2: 91 },
      { title: 'Friday', value1: 22, value2: 73 },
      { title: 'Saturday', value1: 53, value2: 82 },
      { title: 'Sunday', value1: 9, value2: 69 },
    ]
    const progressGroupExample2 = [
      { title: 'Male', icon: 'cil-user', value: 53 },
      { title: 'Female', icon: 'cil-user-female', value: 43 },
    ]
    const progressGroupExample3 = [
      {
        title: 'Organic Search',
        icon: 'cib-google',
        percent: 56,
        value: '191,235',
      },
      { title: 'Facebook', icon: 'cib-facebook', percent: 15, value: '51,223' },
      { title: 'Twitter', icon: 'cib-twitter', percent: 11, value: '37,564' },
      { title: 'LinkedIn', icon: 'cib-linkedin', percent: 8, value: '27,319' },
    ]
    const tableExample = [
      {
        avatar: { src: avatar1, status: 'success' },
        user: {
          name: 'Мария',
          new: true,
          registered: 'Янв 1, 2021',
        },
        country: { name: 'USA', flag: 'cif-us' },
        usage: {
          value: 50,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'success',
        },
        payment: { name: 'Mastercard', icon: 'cib-cc-mastercard' },
        activity: '10 секунд назад',
      },
      {
        avatar: { src: avatar2, status: 'danger' },
        user: {
          name: 'Сергей',
          new: false,
          registered: 'Янв 1, 2021',
        },
        country: { name: 'Brazil', flag: 'cif-br' },
        usage: {
          value: 22,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'info',
        },
        payment: { name: 'Visa', icon: 'cib-cc-visa' },
        activity: '5 минут назад',
      },
      {
        avatar: { src: avatar3, status: 'warning' },
        user: { name: 'Петр', new: true, registered: 'Янв 1, 2021' },
        country: { name: 'India', flag: 'cif-in' },
        usage: {
          value: 74,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'warning',
        },
        payment: { name: 'Stripe', icon: 'cib-cc-stripe' },
        activity: '1 час назад',
      },
      {
        avatar: { src: avatar4, status: 'secondary' },
        user: { name: 'Елена', new: true, registered: 'Янв 1, 2021' },
        country: { name: 'France', flag: 'cif-fr' },
        usage: {
          value: 98,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'danger',
        },
        payment: { name: 'PayPal', icon: 'cib-cc-paypal' },
        activity: 'В течении месяца',
      },
      {
        avatar: { src: avatar5, status: 'success' },
        user: {
          name: 'Светлана',
          new: true,
          registered: 'Янв 1, 2021',
        },
        country: { name: 'Spain', flag: 'cif-es' },
        usage: {
          value: 22,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'primary',
        },
        payment: { name: 'Google Wallet', icon: 'cib-cc-apple-pay' },
        activity: 'На прошлой неделе',
      },
      {
        avatar: { src: avatar6, status: 'danger' },
        user: {
          name: 'Владимир',
          new: true,
          registered: 'Янв 1, 2021',
        },
        country: { name: 'Poland', flag: 'cif-pl' },
        usage: {
          value: 43,
          period: 'Июнь 11, 2021 - Июль 10, 2021',
          color: 'success',
        },
        payment: { name: 'Amex', icon: 'cib-cc-amex' },
        activity: 'На прошлой неделе',
      },
    ]

    return {
      tableExample,
      progressGroupExample1,
      progressGroupExample2,
      progressGroupExample3,
    }
  },
}
</script>


<template>
  <div>
    <div class="py-6 select-none bg-red-500">
      <h1 class="text-xl font-semibold text-center text-white sm:text-2xl">
        <!--The white coloured text rename to desired Main title. will be displayed on the page-->
        Kuching Sentosa Parade Commercial Centre
      </h1>
    </div>
    <div class="max-w-4xl px-2 mx-auto space-y-6 divide-y">
     <!-- Facilities  -->
     <!-- The white coloured text will be displayed on your page. Rename accordingly to your requirements-->
     <!-- Check file components>Design.vue file line 67 for next step-->
      <section  class="py-6 space-y-6">
          <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl">Kuching Sentosa Parade Commercial Centre </h3>
          <section>
      <div class="max-w-6xl px-4 py-12 mx-auto space-y-12">
        <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl text-center">
            
          </h3>
          <!-- You can rename LayoutOneBedroom to your desired variable name
          example: rename "LayoutOneBedroom" on line 27 to "MallLGFloor". DON'T forget to rename LayoutOneBedroom on line 72 to MallLGFloor too
          Do the same to the rest if you are required to rename it. For example "LayoutTwoBedroom" on line 33 and line 79-->
          <Design2 :floor-plan-prop="AtoC" />
        </div>
        <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl text-center">
            AtoC
          </h3>
          <Design2 :floor-plan-prop="CtoK" />
        </div>
        <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl text-center">
            CtoK
          </h3>
          <Design2 :floor-plan-prop="MtoR" />
        </div>
        <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl text-center">
            MtoR
          </h3>
          <Design2 :floor-plan-prop="StoU" />
        </div>
        <div class="space-y-4">
          <h3 class="text-xl font-semibold sm:text-2xl text-center">
            StoU
          </h3>
          <Design2 :floor-plan-prop="UtoZ" />
        </div>
      </div>
    </section>
        </div>
      </section> 
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      //Please rename the title (orange coloured text) and url (orange coloured text) below to the intended title and images
      //the title will be displayed on the page and
      //url needs to use the same name with the name of the pictures you put in the assets>img>create your-own-folder (to hold the pictures)
      //example; for this template, we have a folder named floorlayout. 
      //floorlayout folder have a picture named: Layout1.jpg so the url part below will be url: 'Layout1'
      //so if you create your-own-folder named: shoplots, and import all the pictures into the folder the steps will be the same
      //example: assets>img>shoplots>watson.jpg, the title will be, title: 'Watson' and url will be, url: 'watson' 

      //You can add and remove the number of layout below according to your requirements. 
      //delete the whole line if not needed, and add the whole line if needed. example on LayoutFourBedroom and LayoutFiveBedroom
      AtoC: [
        { title: '24 Hours', floor: 'Ground floor', lot: 'No.1702', url: 'IMG_20230808_092027' },
        { title: '777 Cafe', floor: 'Ground floor', lot: 'No.1695-1696', url: '1691922993123' },
        { title: 'Ah Wu Enterprise Sdn. Bhd', floor: 'Ground floor', lot: 'No.1689', url: '1691922993163' },
        { title: 'Aspec Car Accessories (Wisma Atas)(First two floor,no.1612)', url: 'IMG_20230808_093219' },
        { title: 'Atomy (Kuching Sentosa Prosper Centre)(First floor,no.1621)', url: 'IMG_20230808_092959 Atomy' },
        { title: 'Auto Gard Enterprise (Ground floor,no.1618)', url: 'IMG_20230808_093023 Auto' },
        { title: 'Bank Rakyat (Two floors,no.1654)', url: 'IMG_20230808_092554' },
        { title: 'Batu 8 Mart (Ground floor,no.1688)', url: '1691589854752 Mart' },
        { title: 'BEM (SIB) Olive Garden Church (Two floors,no.1678-1682)', url: '1691917910729' },
        { title: 'Borneo Kedai Serbaneka (Ground floor,no.1700-1701)', url: '1691922993097' },
        { title: 'Charm. S Hair Salon (First floor,no.1619)', url: 'IMG_20230808_093023 Charm' },
        { title: 'CN Beauty Hair Saloon (First floor,no.1677)', url: '1691917910693' },

      ],
      CtoK: [
        { title: 'CS Mini Market (Ground floor,no.1668-1673)', url: 'IMG_20230808_092325' },
        { title: 'D Valley Supermarket (Ground floor,no.1626-1634)', url: '1691589854912' },
        { title: 'Dar Zen Food Centre (Ground floor,no.1635-1637)', url: 'IMG_20230808_092758 Zen' },
        { title: 'Dima Certification Sdn Bhd (First floor,no.1639)', url: 'IMG_20230808_092734 Dima' },
        { title: 'Ding Tea Cafe (Ground floor,no.1656)', url: '1691589854903' },
        { title: 'Gold Mak Hydraulic Seal Kit Centre (First floor,no.1618)', url: 'IMG_20230808_093023 Gold' },
        { title: 'Golden Dragon City Supermarket (Ground floor,no.1690-1694)', url: '1691922993154' },
        { title: 'Guardian (Ground floor,no.1659)', url: '1691589854858' },
        { title: 'Hey Hey Cafe (Ground floor,no.1687)', url: '1691589854752' },
        { title: 'Ho Bi So Food Corner (Ground floor,no.1675-1677)', url: '1691917910693 Ho' },
        { title: 'Klinik Pergigian Eternity Smile (First floor,no.1658)', url: '1691589854846' },
        { title: 'KS Ingredients Sdn.Bhd (Ground floor,no.1619)', url: 'IMG_20230808_093023' },
      ],
      MtoR: [
        { title: 'Master Money Lender Sdn.Bhd (First floor,no.1623)', url: 'IMG_20230808_092944 Master' },
        { title: 'Moms Laksa Cafe (Ground floor,no.1625)', url: 'IMG_20230808_092920' },
        { title: 'Mr D.I.Y: Always Low Prices (First two floor,no.1661)', url: '1691910061702' },
        { title: 'Nena Laundry: Clean & Fresh (Ground floor,no.1638)', url: 'IMG_20230808_092758' },
        { title: 'New Atmosferah Restaurant 4 (Ground floor,no.1685-1686)', url: '1691589854758' },
        { title: 'NK Vape (Ground floor,no.1617)', url: 'IMG_20230808_093039' },
        { title: 'Pasti Jaya Money Lender (First floor,no.1616)', url: 'IMG_20230808_093056' },
        { title: 'Perusahaan Temiang Mutiara Sdn.Bhd (First floor,no.1638)', url: 'IMG_20230808_092758 Perusahaan' },
        { title: 'PES Eco Engineering Sdn.Bhd (First floor,no.1624)', url: 'IMG_20230808_092932 PES' },
        { title: 'Razor Barn Barbershop (For Rent) (First floor,no.1687)', url: '1691589854752 Razorbarn' },
        { title: 'Refresh 88 (For Rent:01135338818)(Ground floor,no.1697)', url: '1691922993115' },
        { title: 'Room for Rent (First floor,no.1689)', url: '1691922993163 Sewa' },
      ],
      StoU: [
        { title: 'Sam Fah (Ground floor,no.1642-1643)', url: '1691910061689' },
        { title: 'Share Tea Cafe (Ground floor,no.1658)', url: '1691910061586' },
        { title: 'Shellemas (Wisma Atas) (Ground floor,no.1613)', url: 'IMG_20230808_093202' },
        { title: 'Silantek Coal Sdn. Bhd (First floor,no.1637)', url: 'IMG_20230808_092758 Silantek' },
        { title: 'Speed Wash 24-Hours Coin Laundry (Ground floor,no.1623)', url: 'IMG_20230808_092944' },
        { title: 'Talent Autoparts Enterprise (Three floors,no.1622)', url: 'IMG_20230808_092959' },
        { title: 'TCC Plastic and Household Sdn. Bhd (First two floors,no.1641)', url: 'IMG_20230808_092734' },
        { title: 'Tealife Cafe (Ground floor,no.1624)', url: 'IMG_20230808_092932' },
        { title: 'The Smart Credit Sdn.Bhd (First floor,no.1625)', url: 'IMG_20230808_092920 Smart' },
        { title: 'Tian Xiang Cafe (Ground floor,no.1698-1699)', url: '1691922993105' },
        { title: 'Tung Yang (Ground floor,no.1678-1682)', url: '1691917910729' },
        { title: 'Unoccupied (Unspecified,no.1614)', url: 'IMG_20230808_093145' },
      ],
      UtoZ: [
        { title: 'Unoccupied (Unspecified,no.1667)', url: 'IMG_20230808_092135' },
        { title: 'Unoccupied (Unspecified,no.1674)', url: 'IMG_20230808_092341' },
        { title: 'Unoccupied (Unspecified,no.1683)', url: 'IMG_20230808_092608' },
        { title: 'Unoccupied (For Rent: 013-8118770/ 0165222164) (First floor,no.1640)', url: 'IMG_20230808_092734 For' },
        { title: 'Unoccupied (For Rent:0193503998) (First floor,no.1685-1686)', url: '1691589854758 Unoccupied' },
        { title: 'Unoccupied (For Sale/ Rent: 1700817669) (Unspecified,no.1657)', url: 'IMG_20230808_092529' },
        { title: 'Unoccupied (Lily Floral & Gift) (Unspecified,no.1620)', url: 'IMG_20230808_092959 Lily' },
        { title: 'Unoccupied (Sheng H Saloon) (Unspecified,no.1611)', url: 'IMG_20230808_093219 Sheng' },
        { title: 'Unoccupied(Persatuan Pencegah T.B Sarawak) (Unspecified,no.1615)', url: 'IMG_20230808_093118' },
        { title: 'Unocupied(For rent: 0128982868) (First floor,no.1656)', url: '1691910061666' },
        { title: 'Unocupied(For rent: 0128982868) (Second floor,no.1656)', url: '1691910061666 Rent' },
        { title: 'V Home:Furniture Concept (Ground floor,no.1609-1610)', url: 'IMG_20230808_093244' },
        { title: 'Wash And Dry (Ground floor,no.1684)', url: '1691917910760' },
        { title: 'Zainab Family Food Court (Ground floor,no.1703)', url: '1691910061600' },
      ],

    }
  },
}
</script>

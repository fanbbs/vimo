<template>
    <Page>
        <Header>
            <Navbar>
                <Title>只有ICON</Title>
            </Navbar>
        </Header>
        <Tabs tabsLayout="title-hide" tabsPlacement="bottom">
            <router-view></router-view>
            <Tab slot="tab" :to="{name:'iconOnly.demoTab1'}" tabBadge="13" tabTitle="User" tabBadgeStyle="danger"
                 tabIcon="person"></Tab>
            <Tab slot="tab" :to="{name:'iconOnly.demoTab2'}" tabBadge="2" tabTitle="Cars" tabBadgeStyle="dark"
                 tabIcon="car"></Tab>
            <Tab slot="tab" :to="{name:'iconOnly.demoTab3'}" tabBadge="7" tabTitle="Star" tabIcon="star"
                 :enabled="true"></Tab>
        </Tabs>
    </Page>
</template>
<style scoped lang="scss"></style>
<script type="text/javascript">
  import { Tabs, Tab } from 'vimo/components/tabs'
  export default{
    name: 'name',
    components: {Tabs, Tab}
  }
</script>

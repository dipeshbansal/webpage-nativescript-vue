<template>
    <Page>
        <ActionBar title="Code Heroku task" />
        <GridLayout columns="*, *, *" rows="*, *, *" width="600" height="600"
            backgroundColor="red">
            <Image class="image" row="0" col="0" 
                src="~/images/StrawberryCropped.jpg" 
                @tap="$navigateTo(detailPage)" />
            <Label class="txt" row="0" col="0" text="Tickets" width="40" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="0" col="1"
                src="~/images/Guitar.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="0" col="1" text="Entertainment"  width="80" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="0" col="2"
                src="~/images/Column.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="0" col="2" text="FAQ" width="40" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="1" col="0"  
                src="~/images/PaintBrushCropped.jpg" 
                @tap="$navigateTo(detailPage)" />
            <Label row="1" col="0" text="Arts & Craft Vendors" width="120" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="1" col="1"
                src="~/images/MapExample.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="1" col="1" text="Festival Map" width="70" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="1" col="2"
                src="~/images/Building.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="1" col="2" text="Museum Info" width="80" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="2" col="0"
				 src="~/images/Strawberry.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="2" col="0" text="Food & Beverage" width="100" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="2" col="1"
                src="~/images/ColumnCropped.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="2" col="1" text="Membership" width="70" height="40"
                verticalAlignment="bottom" />

            <Image class="image" row="2" col="2"
                src="~/images/BuildingCropped.jpg"
                @tap="$navigateTo(detailPage)" />
            <Label row="2" col="2" text="Newsletter Sign-Up" width="120" height="40"
                verticalAlignment="bottom" />
        </GridLayout>
    </Page>
</template>
<script>
    export default {
        data() {
            return {
                detailPage: Webview
            };
        }
    };
    const Webview = {
        template: `
    <Page>
        <ActionBar title="Webview" />
        <StackLayout>
            <WebView height="1200px" src="https://www.nativescript.org" />
          </StackLayout>
        </Page>
      `
    };
</script>
<style scoped>
    .home-panel {
        vertical-align: center;
        font-size: 20;
        margin: 15;
    }

    .description-label {
        margin-bottom: 15;
    }

    .image {
       
        width: 200px;
        position: relative;
        width: 200px;
        height: 200px;
        overflow: hidden;
        border-radius: 50%;
    }

    
</style>
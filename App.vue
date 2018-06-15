<template>
  <!-- <view class="container">
    <text class="text-color-primary">yaya</text>
    <image
          :style="{width: 50, height: 50}"
          :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
    />
    <image
        :style="{width: 66, height: 58}"
        :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
    />
    <text-input
        :style="{borderColor: 'pink', borderWidth: 1}"
        v-model="text"
    />
  </view> -->

  <scrollView :contentContainerStyle="{ paddingVertical: 20 }">
      <text class="text-color-primary">yaya</text>
      <image
            :style="{width: 50, height: 50}"
            :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
      />
      <image
          :style="{width: 66, height: 58}"
          :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
      />
      <text-input
          :style="{borderColor: 'pink', borderWidth: 1}"
          v-model="text"
      />
      <text>lorem*99999999</text>
      <button
        :on-press="onPressLearnMore"
        title="Learn More"
        color="#841584"
        accessibility-label="Learn more about this purple button"
      />
      <activity-indicator size="large" color="#0000ff" />
      <touchable-opacity :on-press="onPressButton">
          <image
            :style="{width: 66, height: 58, marginTop: 100}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
          />
        </touchable-opacity>
    </scrollView>
    <!-- <view style = {styles.container}>
        <image
          :style="{width: 50, height: 50}"
          :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
        />
        <image
            :style="{width: 66, height: 58}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
        /> <image
              :style="{width: 50, height: 50}"
              :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
        />
        <image
            :style="{width: 66, height: 58}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
        /> <image
              :style="{width: 50, height: 50}"
              :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
        />
        <image
            :style="{width: 66, height: 58}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
        /> <image
              :style="{width: 50, height: 50}"
              :source="{uri: 'https://facebook.github.io/react-native/docs/assets/favicon.png'}"
        />
        <image
            :style="{width: 66, height: 58}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
        />
        <switch
            :on-value-change = "handleChange"
            :value = "tootgle" />
        <text>{{tootgle}}</text>

    </view> -->
        <touchable-opacity :on-press="onPressButton">
          <image
            :style="{width: 66, height: 58, marginTop: 100}"
            :source="{uri: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADMAAAAzCAYAAAA6oTAqAAAAEXRFWHRTb2Z0d2FyZQBwbmdjcnVzaEB1SfMAAABQSURBVGje7dSxCQBACARB+2/ab8BEeQNhFi6WSYzYLYudDQYGBgYGBgYGBgYGBgYGBgZmcvDqYGBgmhivGQYGBgYGBgYGBgYGBgYGBgbmQw+P/eMrC5UTVAAAAABJRU5ErkJggg=='}"
          />
        </touchable-opacity>
</template>
<script>
import { Alert } from 'react-native';
export default {
    data: function() {
        return {
            text: 'inputt',
            tootgle: false
        };
    },
    methods: {
        handleChange: () => {
            console.log(!this.tootgle);
            this.tootgle = !this.tootgle
        },
        onPressLearnMore: function() {
            // alert 視窗
            Alert.alert(
                'Alert Title',
                'My Alert Msg',
                [
                    {
                        text: 'Ask me later',
                        onPress: () => console.log('Ask me later pressed')
                    },
                    {
                        text: 'Cancel',
                        onPress: () => console.log('Cancel Pressed'),
                        style: 'cancel'
                    },
                    { text: 'OK', onPress: () => console.log('OK Pressed') }
                ],
                { cancelable: false }
            );
        },
        onPressButton: () => {
            alert('Clicked Image')
        }
    }
};
</script>
<style>
.container {
    background-color: white;
    align-items: center;
    justify-content: center;
    flex: 1;
}
.text-color-primary {
    color: blue;
}
</style>

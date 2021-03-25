<template>
    <div>
        <ams-button label="Change Message" @dostuff="changeMessage"></ams-button>
        <ams-message-display :text="displayText"></ams-message-display>
    </div>
</template>

<script>
//UI Components
import AmsButton from '../shared-components/button/ams-button';
import AmsMessageDisplay from '../shared-components/message/ams-message-display';

//Dependencies
import _randomNumberGenerator from "../shared-components/random-number-generator/random-number-generator";

export default {
    name: "App",
    components: {
        AmsButton,
        AmsMessageDisplay
    },
    data: () => ({
        displayText: "Starting message"
    }),
    methods: {
        changeMessage() {
            var randomNumber = _randomNumberGenerator.getRandomNumber(15,200);
            this.displayText = "A random number is " + randomNumber;
        }
    }
}
</script>
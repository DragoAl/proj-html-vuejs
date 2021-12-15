<template>
    <section>
        <TreatmentCard
        v-for="treatment, i in treatmentsList " :key="i"
        :details='treatment'
        />
    </section>
</template>

<script>
import TreatmentCard from './TreatmentCard.vue'

export default {
    name: 'TreatmentsSection',
    components: {
        TreatmentCard
    },
    data () {
        return {
            treatmentsList: [
                {
                    img: 'Layer-1-new-400x440.jpg',
                    treatName: 'Hydrotherapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-2-new-400x440.jpg',
                    treatName: 'Massage',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-3-new-400x440.jpg',
                    treatName: 'Aromatherapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-4-new-400x440.jpg',
                    treatName: 'Heat Therapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-5-new-400x440.jpg',
                    treatName: 'Skin Care',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-6-new-400x440.jpg',
                    treatName: 'Spa Days',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'layer8-new-400x440.jpg',
                    treatName: 'Beauty Treatments',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-7-new-400x440.jpg',
                    treatName: 'Residential',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
section {
    display: flex;
    flex-wrap: wrap;
   
}

</style>
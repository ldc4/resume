<script>
import { h, provide } from 'vue'

export default {
  name: 'TimeLine',
  setup(props, ctx) {
    provide('timeline', ctx);
    return () => {
      return h(
        'div',
        {
          class: {
            'time-line': true,
          },
        },
        ctx.slots.default?.(),
      )
    }
  },
}
</script>
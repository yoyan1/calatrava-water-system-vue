<!-- Best practice for architecture or design patter -->

1.  components(global component)

    - should only use for shared pages
    - Meaningful: not over specific, not overly abstract.
    - Short: 2 or 3 words.
    - Pronounceable: we want to be able talk about them.
    - PascalCase

      - better to be a dynamic component

      example:
      <!-- recommended -->

      app-header.vue
      user-list.vue
      range-slider.vue

      <!-- avoid -->

      btn-group.vue <!-- short, but unpronounceable. use `button-group` instead -->
      ui-slider.vue <!-- all components are ui elements, so is meaningless -->
      slider.vue <!-- not custom element spec compliant -->

2.  \_components

    - should only per page

3.  Routing

    - routing name should be meaning full
    - use kebab-case
    - 1 or two words only

4.  Version control

    - IMPORTANT! always git fetch and git pull before starting writing your code
    - always branch out for creating pages
    - work on single page only it's ui and bussiness logics
    - always git pull
    - use git conventional naming
    - commit message should be meaningful

5.  Variable

    - same as component naming meaningful
    - camelCase
    - write self documenting code

6.  Format

    - don't use arrow functions ex. const functionName = () => {}
    - script must be in line 1
    - there should be hirearchy in script
      1. state and composables (ref)
      2. getters (computed)
      3. actions (functions)
      4. lifecyle hooks e.g onMounted, watch etc.
    - no abbreviation
    - store should use fetch,add,update,remove and include context or target use plural and singular
    - actions and v-models should be pastensed e.g onSelectChanged, onSumbitted etc.
    - Be explicit about what the action does.

7.  Styling

    - don't use fractional sizes example w-3/2 or w-[60%] (except 100%)
    - don't forget it to make responsive (TBD)
    - consistent spacing, we'll be using 4,8,12,16 etc but for more use case it's okay to not follow

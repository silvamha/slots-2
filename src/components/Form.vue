/**
* Component representing a form.
*
* @slot help - The help content to be displayed above the form.
* @slot fields - The form fields to be displayed.
* @slot buttons - The buttons to be displayed below the form.
*/
<template>
    <form>
        <div class="help">
            <slot name="help"></slot>
        </div>
        <div class="field">
            <slot name="fields"></slot>
        </div>
        <div class="buttons">
            <slot name="buttons"></slot>
        </div>
        <slot></slot>
    </form>
</template>

<!-- <script>
export default {
    name: 'Form'
}

</script> -->

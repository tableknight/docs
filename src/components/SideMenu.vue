<template>
    <q-list separator>
      <q-collapsible indent icon="mail" label="Inbox">

        <q-collapsible indent icon="receipt" label="Receipts"></q-collapsible>

        <q-collapsible indent icon="schedule" label="Postponed">
          <div>{{ lorem }}</div>
        </q-collapsible>

      </q-collapsible>

      <q-collapsible indent icon="send" label="Outbox" sublabel="Empty">
        <q-collapsible label="Today">
          <div>{{ lorem }}</div>
        </q-collapsible>
        <q-collapsible label="Yesterday">
          <div>{{ lorem }}</div>
        </q-collapsible>
      </q-collapsible>

      <q-collapsible indent icon="drafts" label="Draft" sublabel="Draft a new email">
        <div>{{ lorem }}</div>
      </q-collapsible>
    </q-list>
</template>

<script>
    export default {
        data() {
          return {
            lorem: "123"
          }
        },
    }
</script>


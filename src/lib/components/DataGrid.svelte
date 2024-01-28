<script lang="ts">
    import * as Table from "$lib/components/ui/table";
</script>

<div class="">
    <Table.Root>
        <Table.Header>
          <Table.Row>
            <Table.Head class="w-[100px]">type</Table.Head>
            <Table.Head>file name</Table.Head>
            <Table.Head>file size</Table.Head>
            <Table.Head>date added</Table.Head>
            <Table.Head>link</Table.Head>
            <Table.Head class="sr-only" >delete</Table.Head>
          </Table.Row>
        </Table.Header>
        <Table.Body>
          {#each {length:5} as _}
            <Table.Row>
              <Table.Cell class="font-medium">invoice.Invoice</Table.Cell>
              <Table.Cell>invoice.paymentStatus</Table.Cell>
              <Table.Cell>invoice.paymentMethod</Table.Cell>
              <Table.Cell class="text-right">invoice.totalAmount</Table.Cell>
            </Table.Row>
          {/each}
        </Table.Body>
      </Table.Root>
</div>
<template>
    <div>
      <div class="">
        <Accordion type="single" collapsible>
          <AccordionItem value="item-1" class="py-2 px-2">
            <div class="flex justify-between">
              <div class="flex gap-4 items-center">
                <AccordionTrigger class=""> </AccordionTrigger>
                <p>Introduct To The COurse (10 Minutes).</p>
              </div>
              <div>
                <span>4 Leccture.10min</span>
              </div>
            </div>
  
            <AccordionContent> </AccordionContent>
          </AccordionItem>
        </Accordion>
      </div>
    </div>
  </template>
  
  <script setup>
  import {
    Accordion,
    AccordionContent,
    AccordionItem,
    AccordionTrigger,
  } from "./ui/accordion/index.ts"; 
  
  defineProps({
    course: {
      type: Object,
      required: true,
    },
  });
  </script>
  